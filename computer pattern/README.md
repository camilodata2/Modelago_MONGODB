# computed pattern
Es realizar solo los computos necesarios cuando hay cambios, para no calcularlos durante las consultas.
## 💙 caso de uso

  No recalcular en cada consulta, ya que se actualiza cuando es necesario. Pre-calculo para consultas.
  Reduce las consultas necesarias y simplifica las consultas, a costa de las actualizaciones.
  Cuando necesitas calcular un valor a partir de otros campos en un documento y mostrar el resultado en una consulta o informe.
  Cuando es más frecuente la lectura que la escritura.
  Calcular el valor por cada lectura es costoso, es mejor pre calcular en cada escritura.
  No requiere hacer busquedas innecesarias de valores ya agregados, ya que puede ser incremental.
  Se puede manipular con un lenguaje de programacion.

### Ejemplo
Se hara una orden de compra dinamica, en donde, al agregar productos a la orden esta actualizara el valor total que es la suma de todos los productos multiplicado su cantidad.

<img src="https://webassets.mongodb.com/_com_assets/cms/cpucomputed-fbcpkmvbsy.png" alt="Descripción de la imagen" width="300">
