# Análisis de Compras en Instacart

Este proyecto se centra en el análisis de datos de pedidos de la plataforma de compras en línea Instacart, con el objetivo de obtener información valiosa sobre el comportamiento de compra de los clientes. Utilizamos técnicas de análisis de datos y visualización para descubrir patrones y responder a preguntas específicas sobre los datos.

## Índice

1. [Introducción](#intro)
2. [Diccionario de Datos](#data-dictionary)
3. [Principales Hallazgos](#key-findings)
4. [Implicaciones para el Negocio](#business-implications)
5. [Acceso a los Datos](#data-access)

## Introducción <a id='intro'></a>

El análisis de datos realizado en este proyecto nos permitió identificar tendencias clave y patrones en el comportamiento de compra de los usuarios de Instacart. Los resultados obtenidos pueden ser utilizados para mejorar la experiencia del cliente, optimizar la logística y desarrollar estrategias de marketing más efectivas.

## Diccionario de Datos <a id='data-dictionary'></a>

### Tabla: `instacart_orders.csv`
Cada fila corresponde a un pedido en la aplicación Instacart.

- **order_id**: Número de ID que identifica de manera única cada pedido.
- **user_id**: Número de ID que identifica de manera única la cuenta de cada cliente.
- **order_number**: El número de veces que este cliente ha hecho un pedido.
- **order_dow**: Día de la semana en que se hizo el pedido (0 si es domingo).
- **order_hour_of_day**: Hora del día en que se hizo el pedido.
- **days_since_prior_order**: Número de días transcurridos desde que este cliente hizo su pedido anterior.

### Tabla: `products.csv`
Cada fila corresponde a un producto único que pueden comprar los clientes.

- **product_id**: Número ID que identifica de manera única cada producto.
- **product_name**: Nombre del producto.
- **aisle_id**: Número ID que identifica de manera única cada categoría de pasillo de víveres.
- **department_id**: Número ID que identifica de manera única cada departamento de víveres.

### Tabla: `order_products.csv`
Cada fila corresponde a un artículo pedido en un pedido.

- **order_id**: Número de ID que identifica de manera única cada pedido.
- **product_id**: Número ID que identifica de manera única cada producto.
- **add_to_cart_order**: El orden secuencial en el que se añadió cada artículo en el carrito.
- **reordered**: 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.

### Tabla: `aisles.csv`
- **aisle_id**: Número ID que identifica de manera única cada categoría de pasillo de víveres.
- **aisle**: Nombre del pasillo.

### Tabla: `departments.csv`
- **department_id**: Número ID que identifica de manera única cada departamento de víveres.
- **department**: Nombre del departamento.

## Principales Hallazgos <a id='key-findings'></a>

1. **Distribución del Número de Órdenes por Cliente**:
   - La mayoría de los clientes realizan un número relativamente bajo de pedidos, con una disminución significativa a medida que aumenta el número de órdenes.

2. **Tasa de Repetición de Pedidos por Producto**:
   - Los productos con una alta tasa de repetición son aquellos que los clientes compran repetidamente, lo que puede indicar una alta satisfacción o necesidad continua.

3. **Productos Más Vendidos**:
   - Los productos más vendidos incluyen principalmente productos orgánicos y básicos, como "banana", "bag of organic bananas" y "organic whole milk".

4. **Artículos Añadidos Primero al Carrito**:
   - Los productos que se agregan primero tienden a ser esenciales o de alta prioridad para los clientes, como "banana" y "organic whole milk".

5. **Distribución de Pedidos por Hora y Día**:
   - Los pedidos tienden a concentrarse en ciertas horas del día, como a media mañana y en la tarde, y varían entre días de semana y fines de semana.

## Implicaciones para el Negocio <a id='business-implications'></a>

- **Estrategias de Marketing**: Los productos más vendidos y los que se agregan primero al carrito pueden ser el foco de campañas de marketing y promociones.
- **Gestión de Inventarios**: Comprender los patrones de compra y las horas pico puede ayudar a optimizar la gestión de inventarios y la planificación de la cadena de suministro.
- **Mejora de la Experiencia del Cliente**: Conociendo las preferencias de los clientes, Instacart puede personalizar recomendaciones y mejorar la experiencia del usuario en la plataforma.

## Acceso a los Datos <a id='data-access'></a>

Los archivos CSV utilizados en este análisis están disponibles para su consulta y descarga en el siguiente enlace de Google Drive:

[Enlace a los datos en Google Drive](https://drive.google.com/drive/folders/1bv2ULEXNtgHG0zYjmAH1tEDUAimnHB01?usp=sharing)
