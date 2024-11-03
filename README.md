# AAR-Excel-cafeter-a
Ejercicio Excel sobre datos de cafetería

Dos análisis diferentes:
1. Horas y días de la semana con más actividad viendo los productos que se venden por hora para analizar el personal que necesito por turno.

2. Análisis por tienda y tipos de productos más comprados para analizar el comportamiento de los clientes y pensar una estrategia comercial.


Líneas de trabajo:

1. En primer lugar se realizó una primera vista a los datos en los que, a simple vista se vió que había dos transacciones exactamente 
iguales que se procedieron a limpiar y una columna muy necesaria para un buen EDA. La columna "Total Revenue" calculada como los productos
comprados multiplicados por su precio. También se añadieron otras columnas (las que tienen título verde dentro de la pestaña "tratado") para
poder analizar mejor los datos.

2. Se realizó un EDA numérico y categórico en los cuales se observaron a simple vista varios datos importantes: 
	- Nuestros clientes nos compran de media 1 producto (1,44 exactamente) y el ticket medio es de 4,69€ (el rango de precios va de 0,8 a 45)
	- La mediana y la moda de los precios unitarios de los productos vendidos es 3.
	- Las ventas por tienda crecen mes a mes lo cual sugiere que las tres tiendas pueden ser tiendas abiertas en enero que están cogiendo
	  tracción en ventas.
	- El 50% aproximadamente de nuestras ventas está en el turno del desayuno (de 6 a 11 de la mañana)
	- La distribución del tipo de productos vendidos es muy similar en las tres tiendas
	- Se encontraron números de transacciones perdidas aunque solo es un 0,2% que consideramos irrelevante.
   Teniendo en cuenta estos datos, se pueden extraer varias conclusiones:
	- La gran parte de nuestros clientes nos compran un solo producto y de los más baratos, principalmente un té, un café o un chocolate
	  (entre los tres hacen más de un 70% de la facturación total).
	- Por tanto, la empresa podría intentar mejorar los productos complementarios a estos tres como pueden ser los productos de bakery (solo 
	  suponen el 10% de las ventas)
	- Las tiendas tienen una distribución en ventas por turnos, productos, día y mes muy similares. Sería interesante ver si la localización de
	  las tiendas es muy cercana entre ellas. Esto podría ser un indicio de fraude o error en los datos si la localización es diferente entre ellas.

3. Se decide realizar el EDA de correlación a pesar de que solo hay tres datos númericos: cantidad de producto vendido, precio de producto y total transacción
   que obviamente están relacionadas entre si. la correlación entre el total de ventas por transacción es positiva respecto a la cantidad de productos 
   vendidos y muy positiva respecto al precio unitario mientras que la correlación entre las unidades vendidas y su precio es negativa por lo que este dato
   sigue con la línea de que nos compran los productos más baratos.

4. Se seleccionan los KPIs clave según nuestro objetivo:
	- Total transacciones (contar el número de transacciones que tenemos), total productos vendidos (suma de la cantidad de producto por transaccion) y 
          total ingresos (suma de todas las ventas) para hacernos una idea a nivel macro del volumen del negocio que estamos analizando.
	- Media en euros por transacción y media en productos por transacción para ver el comportamiento del cliente 
	- Hora punta para hacernos una idea rápida de cuando tenemos más transacciones en el negocio.

5. Se realiza un dashboard con los KPIs seleccionados y varias gráficas que nos indican la distribución de las ventas por tienda y producto y la evolución del
   número de pedidos por turno, mes y día.

6. Conclusiones:
	-Parece que la distribución por días es bastante similar sin embargo si cambia por turnos. La empresa debería centrar su personal en las horas de las 6 de la
	 mañana a las 11, especialmente de 10 a 11 que es la hora punta en todas las tiendas y analizar si puede ser rentable cerrar la tienda antes ya que son las 
	  horas en las que menos clientes tenemos.
	- En cuanto al análisis de las ventas, parece que nuestros clientes compran solo un producto y que suele ser una bebida. La empresa podría centrar su estrategia
	  en no perder la calidad de sus cafés tés y chocolates y mejorar la oferta y calidad de productos complementarios como pueden ser los de la categoría bakery. 
	- Visto el avance que están teniendo en ventas las tiendas y que sus productos más vendidos, según la lógica al ser productos calientes, deberían venderse más 
	  en épocas de frío, podría ser interesante abrir nuevas tiendas de cara a octubre o noviembre en zonas similares.

7. Next Steps:
	-  La distribución muy similar de los números de transacciones por tienda y día puede sugerir que haya fraude o error en la recoleción de los datos. Ase-
	   gurar que esto es correcto y que concuerda con la ubicación de las tiendas.
	-  Hacer un análisis de la rentabilidad de los productos añadiendo datos como el coste unitario por producto y fecha para analizar la rentabilidad de cada
	   producto. Lo he intentado analizar con datos de Chat GPT pero daba rangos muy amplios. 
	-  Continuar con la recolección de los datos para ver el avance.

