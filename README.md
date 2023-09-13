## **🍷 Vinografo:** Un enfoque Data-Driven para comprender la calidad del vino.

## 🔎 Tabla de Contenidos
* 🤯 ¿Cuál es la necesidad o problema a resolver?

* 🏢 Consultas del negocio

* 📊 Base de datos

* 👉 Descripción de las variables

* 🍷 Conclusiones finales

## 🤯¿Cuál es la necesidad o problema a resolver? 

La calidad del vino es influenciada por una variedad de factores, como sus propiedades químicas y características organolépticas. Resolver el desafío de identificar la relación entre estos factores y la calidad del vino nos permitirá no solo comprender mejor los matices que influyen en su sabor y percepción, sino también tener una visión más completa de la complejidad detrás de esta apreciada bebida y la experiencia del consumidor.   
Además, al comparar vinos blancos y tintos en términos de calidad, podemos descubrir patrones específicos asociados con cada tipo y arrojar luz sobre posibles diferencias en sus procesos de elaboración.

## 🏢 Preguntas del negocio:
1. ¿Entre vino blanco y tinto, qué tipo tuvo mejor calificación en calidad?
2. ¿Existe una relación entre cada factor y la calidad del vino?
3. ¿Cuál es la influencia de la concentración de alcohol en la calidad del vino y cómo se compara esta influencia entre vinos blancos y tintos? 

## 📊 Base De Datos:

Fuente:  
[Wine Quality Data Set Red & White Wine](https://www.kaggle.com/datasets/ruthgn/wine-quality-data-set-red-white-wine)

**Descripción del dataset:**
Este conjunto de datos contiene información de 1599 muestras de vino tinto y 4898 muestras de vino blanco.
Debido a problemas de privacidad y logística, no hay datos sobre los tipos de uva, la marca del vino y el precio de venta del vino.


## 👉 Descripción de las variables

Las variables de entrada en el conjunto de datos consisten en el tipo de vino (ya sea vino tinto o vino blanco) y métricas de pruebas objetivas (por ejemplo, niveles de acidez, valores de pH, contenido alcohólico, etc.), mientras que la variable objetivo/salida es una puntuación numérica basada en datos sensoriales, que es la mediana de al menos 3 evaluaciones realizadas por expertos en vinos (En una escala del 0 - muy malo a 10 - excelente).

Para esta consultoría nos enfocaremos en las siguientes 5 variables que comunmente se cree tienen mayor influencia en la calidad percibida del vino:

* **Tipo de vino:** El tipo de vino, ya sea tinto o blanco, es uno de los factores más influyentes, ya que afecta fundamentalmente el perfil de sabor, aroma y estructura del vino.  
* **Acidez fija:** La acidez fija es crucial para la frescura y la viveza del vino. Una acidez equilibrada puede realzar los sabores y mantener el vino en equilibrio.  
* **Azúcar residual:** El nivel de azúcar residual afecta directamente la percepción de dulzura del vino, lo cual puede tener un impacto importante en cómo se percibe el vino en términos de equilibrio y gusto.  
* **pH:** El pH influye en la acidez y la sensación en boca del vino. Un pH adecuado es esencial para mantener la frescura y el equilibrio en el vino.  
* **Alcohol:** El contenido de alcohol afecta la sensación en boca, la intensidad de los sabores y la estructura del vino. Un equilibrio adecuado es esencial para lograr una experiencia agradable.  

## **Respondiendo las preguntas:** 

❓ **¿Entre vino blanco y tinto, qué tipo tuvo mejor calificación en calidad?**  
Para esto, utilizaremos las funciones **counts_with_type**, **totals_by_type**, y **percentages_with_type** para calcular los conteos de cada combinación de **'type'** y **'quality_category'**, así como los totales por tipo de vino, los porcentajes para cada tipo de vino y agregar una columna que muestre el total por tipo de vino.

❓ **¿Existe una relación entre cada factor y la calidad del vino?**  
Con correlation_matrix  básicamente estamos calculando algo llamado **"coeficiente de correlación"** utilizando nuestro conjunto de datos **df_vinografo**. Lo que estamos haciendo es ver cómo todas nuestras variables numéricas se relacionan con la columna **'quality'**. La matriz resultante nos dará una idea de si hay alguna relación entre estas variables y la calidad del vino. Después de hacer todos estos cálculos, simplemente mostramos o imprimimos esa matriz de correlación.  

❓ **¿Cuál es la influencia de la concentración de alcohol en la calidad del vino y cómo se compara esta influencia entre vinos blancos y tintos?**  
Aquí agrupamos nuestros datos por tipo de vino usando **groupby**, luego calculamos la correlación entre el contenido de alcohol y la calidad del vino para cada tipo usando una función especial y, por último, mostramos los resultados de esas correlaciones.  


## **🍷 Conclusiones** 

**En este análisis, se evalúa la relación entre 5 variables y la calidad de los vinos blancos y tintos.**

* Observamos que la variable 'alcohol' parece estar más fuertemente relacionada con la calidad del vino en comparación con las otras variables, que tienen correlaciones más débiles y podrían no ser tan influyentes en la calidad percibida del vino en este conjunto de datos.
* La correlación entre el alcohol y la calidad varía según el tipo de vino.  
* En el caso de los vinos tintos, encontramos una correlación positiva significativa entre el alcohol y la calidad, lo que sugiere que un mayor contenido de alcohol tiende a asociarse con una mejor calidad en estos vinos.  
* Por otro lado, en los vinos blancos, la correlación es menos pronunciada y podría indicar que la calidad de los vinos blancos está influenciada por otros factores en mayor medida.  
* Estas diferencias subrayan la importancia de considerar el tipo de vino al evaluar la influencia de los componentes químicos en su calidad, lo que puede ser relevante para la producción y selección de vinos de alta calidad.  
