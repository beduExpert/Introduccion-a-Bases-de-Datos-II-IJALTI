[`Introducción a Bases de Datos`](../README.md) > `Sesión 3`

## Sesión 3: Agregaciones

<img src="../imagenes/pizarron.png" align="right" height="100" width="100" hspace="10">
<div style="text-align: justify;">

### 1. Objetivos :dart: 

- Repasar qué es una agregación y una capa
- Analizar las agregaciones de agrupamiento
- Generar vistas que almacenen el resultado de una agregación

### 2. Contenido :blue_book:

---
#### <ins>Agrupamientos</ins>
<img src="imagenes/imagen1.jpg" align="right" height="200" width="300">

Al igual que en __SQL__ en __MongoDB__ podemos realizar agrupamientos. Se realizan mediante la agregación `$group` y tienen la siguiente sintaxis:

```json
{
  $group:
    {
      _id: <expression>, // Group By Expression
      <field1>: { <accumulator1> : <expression1> },
      ...
    }
 }
```

- [**`EJEMPLO 1`**](Ejemplo-01/Readme.md)
- [**`RETO 1`**](Reto-01/Readme.md)

---
#### <ins>Asociación de colecciones</ins>
<img src="imagenes/imagen2.jpg" align="right" height="200" width="300">

De la misma forma en que __SQL__ incluye distintos tipos de *join*. En __MongoDB__ se tiene la operación `$lookup` que permite relacionar colecciones. Es una agregación y su sintaxis es la siguiente:

```json
{
   $lookup:
     {
       from: <collection to join>,
       localField: <field from the input documents>,
       foreignField: <field from the documents of the "from" collection>,
       as: <output array field>
     }
}
```

- [**`EJEMPLO 2`**](Ejemplo-02/Readme.md)
- [**`RETO 2`**](Reto-02/Readme.md)	

---
#### <ins>Generación de vistas</ins>
<img src="imagenes/imagen3.png" align="right" height="150" width="150">

En __MongoDB__ también es posible generar vistas que almacenen el resultado de las distintas consulas. Para generar una vista usaremos __Compass__.

Una vez creada la vista, podemos consultarla como a cualquier otra colección.

- [**`EJEMPLO 3`**](Ejemplo-03/Readme.md)
- [**`RETO 3`**](Reto-03/Readme.md)

---

### 3. Ejercicios :hammer:

Aplica lo todo lo que aprendiste durante la sesión con estos ejercicios.

- [**`EJERCICIOS SESIÓN 7`**](Ejercicios/Readme.md)


### 4. Postwork :memo:
Aplica lo todo lo que aprendiste durante la sesión a tu proyecto personal.

- [**`POSTWORK SESIÓN 7`**](Postwork/Readme.md)

</br>

[`Anterior`](../Sesion-05/Readme.md) | [`Siguiente`](../Sesion-07/Readme.md)

</div>	
