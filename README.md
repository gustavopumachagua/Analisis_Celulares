# **Análisis de productos en Amazon con web scraping**

---

![Amazon!](./img/amazon.png "Amazon")

---

- [Extracción de datos de la pagina web de amazon con web scraping con python](#extracción-de-datos-de-la-pagina-web-de-amazon-con-web-scraping-con-python)

  - [Nomenclatura de los datos](#nomenclatura-de-los-datos)

- [Limpiar y Filtrar los datos mas relevantes](#limpiar-y-filtrar-los-datos-mas-relevantes)

- [Estadisticas y Transformacion de los datos](#estadisticas-y-transformacion-de-los-datos)

---

## **Extracción de datos de la pagina web de amazon con web scraping con python**

El Siguiente proyectos se basa extraer los datos de la pagina web se Amazon por medio de Web Scraping.

Los Datos seran las Laptops de ofrece Amazon. lo encontrará [aquí](https://www.amazon.com/s?i=computers-intl-ship&bbn=16225007011&rh=n%3A16225007011%2Cn%3A13896617011%2Cn%3A565108&dc&language=es&ds=v1%3AvpurCweVslklayCwT4TrkFrW2VBuk2iGhJ82EII4vmE&qid=1679180569&rnid=13896617011&ref=sr_nr_n_2 "Laptops").

El procedimiento para la extracción de datos para un análisis de la página web de Amazon utilizando web scraping con Beautiful Soup en Python es el siguiente:

- **Instalar Beautiful Soup:**

Primero, debe asegurarse de tener instalada la biblioteca Beautiful Soup. Puede instalarla utilizando pip en su terminal de comando, por ejemplo: pip install beautifulsoup4.

- Identificar la URL de la página web de Amazon que contiene los datos que se desean extraer.

- **Inspeccionar la página web:**

Abra la página web en su navegador y use las herramientas de desarrollador del navegador para inspeccionar los elementos HTML de la página y encontrar los elementos que contienen los datos que desea extraer.

- **Crear una solicitud HTTP:**

Utilice la biblioteca Requests para enviar una solicitud HTTP a la URL de la página web que desea extraer. Esto le permitirá obtener el contenido HTML de la página web.

- **Crear un objeto Beautiful Soup:**

Utilice Beautiful Soup para analizar el contenido HTML y crear un objeto de tipo Beautiful Soup. Esto le permitirá extraer datos específicos del contenido HTML.

- **Extraer datos específicos:**

Utilice las funciones de Beautiful Soup para extraer datos específicos de los elementos HTML que identificó previamente en la página web. Por ejemplo, puede usar la función find o find_all para buscar elementos HTML específicos por su etiqueta, clase o atributo.

- **Almacenar los datos extraídos:**

Almacene los datos extraídos en una estructura de datos adecuada, como un diccionario o una lista, para su posterior análisis.

- **Procesar los datos extraídos:**

Limpie y procese los datos extraídos según sea necesario, como convertir los precios en números, eliminar caracteres no deseados, etc.

- **Automatizar el proceso:**

Utilice bucles y la función de paginación para automatizar el proceso de extracción de datos y recopilar datos de varias páginas web en Amazon.

---

![Web Scraping!](./img/web%20scraping.png "Web Scraping")

---

### **Nomenclatura de los datos**

Para hacer gráficos estadísticos para un análisis de la página web de Amazon utilizando web scraping con Python, se necesitarán extraer datos relevantes de la página web. Algunos de los datos que pueden ser relevantes para el análisis incluyen:

- **Product:**

  Nombre del producto.

- **Price_Now:**

  Precio Despues de aplicarle el descuento.

- **Price_Before:**

  Precio sin aplicarle el descuento.

- **Stock:**

  Cantidad de Unidades almacenada.

- **Rating:**

  Apreciacion de los productos el rango es [0-5]

- **Voters:**

  Cantidad de persona que dieron su apreciacion a los productos.

- **Category:**

  Las diferentes marcas que pertenece los productos.

- **Qualification %**

  Se calcula: [(Ranting) / 5] \* 100%

  Ranting_Maximo = 5

- **Discounts %**

  Se calcula: [(Price_Before - Price_Now) / Price_Before] \* 100%

[🔼](#análisis-de-productos-en-amazon-con-web-scraping)

---

## **Limpiar y Filtrar los datos mas relevantes**

- **Eliminar valores duplicados:**

Los datos duplicados pueden introducir errores en el análisis y deben eliminarse.

- **Revisar valores faltantes:**

Si hay valores faltantes, debe determinarse si es posible imputarlos o si deben eliminarse las filas correspondientes.

- **Verificar la consistencia de los datos:**

Los valores extremos o inesperados pueden ser señal de errores en la recolección de datos y deben verificarse y, si es necesario, corregirse.

- **Verificar la calidad de los datos:**

Los datos incompletos, inconsistentes o incorrectos pueden ser una señal de problemas en la calidad de los datos y deben ser corregidos.

- **Normalizar los datos:**

Los valores de los datos pueden estar en diferentes escalas o unidades, lo que puede dificultar la comparación entre ellos. Es posible que deba normalizar los datos para facilitar el análisis.

- **Verificar la precisión de los datos:**

los errores de entrada de datos pueden introducir errores en el análisis. Por lo tanto, debe verificar que los datos se ingresaron correctamente y hacer correcciones si es necesario.

- **Estandarizar los datos:**

Los nombres de columnas o variables pueden variar en diferentes conjuntos de datos. Para facilitar el análisis, es posible que deba estandarizar los nombres de las variables.

[🔼](#análisis-de-productos-en-amazon-con-web-scraping)

---

## **Estadisticas y Transformacion de los datos**

- **Histograma de precios:**

Puedes crear un histograma que muestre la distribución de precios de tus productos. Esto puede ayudarte a identificar el rango de precios más común y a entender cómo se comparan tus productos en términos de precio.

- **Gráfica de barras de descuentos:**

Puedes crear una gráfica de barras que muestre la cantidad de productos que tienen diferentes niveles de descuento. Esto puede ayudarte a entender cómo los descuentos afectan las ventas de tus productos y a identificar qué productos tienen los mayores descuentos.

- **Gráfica de dispersión de ranking y votos:**

Puedes crear una gráfica de dispersión que muestre el ranking de tus productos en Amazon en función del número de votantes. Esto puede ayudarte a entender la relación entre la popularidad de tus productos y su ranking en Amazon.

- **Gráfica de líneas de stock:**

Puedes crear una gráfica de líneas que muestre cómo cambia el stock de tus productos con el Descuentos. Esto puede ayudarte a planificar mejor tus inventarios y a evitar quedarte sin stock de tus productos.

- **Gráfica de barras de porcentaje de ranking:**

Puedes crear una gráfica de barras que muestre el porcentaje de productos que tienen diferentes rangos de ranking. Esto puede ayudarte a entender cómo se comparan tus productos en términos de ranking y a identificar los productos que tienen los mejores y peores rangos de ranking.

[🔼](#análisis-de-productos-en-amazon-con-web-scraping)

---
