# Taller · Las cinco funciones de partida

| # | Función             | ¿Qué muta la versión de TypeScript?                                                        | ¿Quién más se entera del cambio?                                                                                              |
| - | ------------------- | ------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| 1 | `total_pesos`       | Muta la variable `total` en cada vuelta del `for`, sumándole el `pesoKg` de cada embarque. | Nadie fuera de la función, porque `total` es una variable local.                                                              |
| 2 | `marcar_urgentes`   | Muta cada objeto `Embarque`, modificando su propiedad `urgente`.                           | Cualquier código que tenga una referencia a esos mismos objetos, porque los objetos originales fueron modificados.            |
| 3 | `aplicar_descuento` | Muta el arreglo `precios`, cambiando directamente cada elemento `precios[i]`.              | Cualquier código que tenga una referencia al mismo arreglo `precios`, porque el arreglo original fue modificado.              |
| 4 | `contar_por_tipo`   | Muta el objeto `conteo`, agregando o incrementando propiedades para cada tipo de embarque. | Nadie fuera de la función mientras se está construyendo, porque `conteo` es local; los demás solo reciben el resultado final. |
| 5 | `sin_duplicados`    | Mutan `vistos` y `resultado`: `vistos` agrega IDs y `resultado` agrega IDs únicos.         | Nadie fuera de la función, porque ambas estructuras son creadas dentro de la función y son locales.                           |
