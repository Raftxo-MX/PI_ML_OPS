<h1 align=center>🚀🚀🚀 **PROYECTO INDIVIDUAL Nº1** 🚀🚀🚀</h1>
<h2 align=center> Alumno: Rafal Janusz Wysocki raftxo.mx@gmail.com </h2>
<h1 align=center>**`Machine Learning Operations (MLOps)`**</h1>

<br><hr>

<p align=center style='background-color:#333333;font-size:large;font-style:italic' >
El que al viento observa, no sembrará; y el que mira a las nubes, no segará. <sub>Eclestiastés 11:4</sub>
</p>

### **`Ingeniería de datos`**:  

En la primera etapa [**`Data Engineer`** **`MVP`** (_Minimum Viable Product_)] procedemos a la ingesta de datos proporcionados en dos archivos .CSV `movies_dataset.csv` y `credits.csv`, su tratamiento (transformación) consistente en buscar duplicados, nulos, etc... para poder finalmente devolver un conjunto de datos limpios en un solo archivo. En mi caso el archivo resultante se llama `datos_limpios.csv`.
Todos estos procesos al igual que el desarrolo de las primeras funciones de la API están disponibles para su lectura en el archivo ETL_pi01_dts12.ipynb dentro del presente repositorio.  
>https://github.com/Raftxo-MX/PI_ML_OPS/blob/main/ETL_pi01_dts12.ipynb



<br/>

### **`Desarrollo API`**:
En esta etapa procedemos a desarrollar las funciones requeridas y el despliegue de la API en Render usando FastAPI. Los archivos utilizados en el despliegue están en un repositorio por separado.

>https://github.com/Raftxo-MX/faster - el repositorio  
>https://github.com/Raftxo-MX/faster/main.py - el archivo main.py con las funciones

<br/>

### **`Machine Learning`**:  
En esta etapa procedemos al análisis exploratorio del conjunto de datos limpio, seleccionamos las columnas adecuadas para implementar el sistema de recomendaciones.  

Hemos usado Extracción Automática de Palabras Clave Relevantes (RAKE) para generar conjuntos de palabras clave para cada película basados en la columna 'overview'. El mismo algoritmo también genera puntajes de palabras clave (keyscores) que seguidamente se han comparado usando la similitud cosinusoide.

Para la entrega del producto mínimo víable optamos por generar en local, a través del modelo ML, un conjunto de datos con las recomendaciones y usarlo en la API aligerando así enormemente su funcionamiento. Si más adelante, el cliente quiere desplegar todo el potencial del modelo online, necesitaríamos un servicio web con más recursos. El mismo Render en sus opciones de paga, nos serviría.

>https://github.com/Raftxo-MX/PI_ML_OPS/blob/main/ML_pi01_dts12.ipynb - el desarrollo del modelo 

<br/>

### **`MVP`** (_Minimum Viable Product_)]

A continuación se proporcionan enlaces de comprobación de la API desplegada. 

>https://fastapirender.onrender.com/  - despliegue de la API  
>https://fastapirender.onrender.com/docs - interfaz gráfica de FastAPI
>https://fastapirender.onrender.com/peliculas_duracion/What%20the%20%23%24%2A%21%20Do%20We%20%28K%29now%21%3F    

<br/>  

>https://youtu.be/cL7_Awn8JWM - Enlace al vídeo explicativo del proyecto


<p align=center style='background-color:#333333;font-size:large;font-style:italic' >
"Una gran aventura puede comenzar con un pequeño paso. 😉" <sub>Summer Smith, Rick & Morty</sub>
</p>

## **Fuente de datos**

+ [Dataset](https://drive.google.com/drive/folders/1nvSjC2JWUH48o3pb8xlKofi8SNHuNWeu): Carpeta con los 2 archivos con datos que requieren ser procesados (movies_dataset.csv y credits.csv), tengan en cuenta que hay datos que estan anidados (un diccionario o una lista como valores en la fila).
+ [Diccionario de datos](https://docs.google.com/spreadsheets/d/1QkHH5er-74Bpk122tJxy_0D49pJMIwKLurByOfmxzho/edit#gid=0): Diccionario con algunas descripciones de las columnas disponibles en el dataset.
<br/>

## **Material de apoyo**

+ [links de ayuda](hhttps://github.com/HX-PRomero/PI_ML_OPS/raw/main/Material%20de%20apoyo.md). 
+ [artículo sobre EDA](https://medium.com/swlh/introduction-to-exploratory-data-analysis-eda-d83424e47151)
+ [diagrama conceptual procesos del proyecto](https://github.com/HX-PRomero/PI_ML_OPS/raw/main/src/DiagramaConceptualDelFlujoDeProcesos.png)
+ [consideraciones de un MVP aprobatorio](https://github.com/HX-PRomero/PI_ML_OPS/raw/main/src/MVP_MLops.PNG)
  
<br/><br/><br/><br/><br/>

<!--
<style>
/* Estilo para ocultar el texto dentro de los comentarios */
comment {
  display: none;
}
</style>

😉

NOTA: Recuerde entregar el link de acceso al video. Puede alojarse en YouTube, Drive o cualquier plataforma de almacenamiento. **Verificar que sea de acceso público, recomendamos usar modo incógnito en tu navegador para confirmarlo**.

<br/>
Aqui te sintetizamos que es lo que consideramos un MVP aprobatorio, y la diferencia con un producto completo.



<p align="center">
<img src="https://github.com/HX-PRomero/PI_ML_OPS/raw/main/src/MVP_MLops.PNG"  height=250>
</p>




FIN DE OCULTAMIENTO DE TEXTO. -->
