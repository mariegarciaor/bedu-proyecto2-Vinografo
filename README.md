## **🍷 Vinografo:** Un enfoque Data-Driven para comprender la calidad del vino.

## 🔎 Tabla de Contenidos
-🤯 ¿Cuál es la necesidad o problema a resolver?

-🏢 Consultas del negocio

-📊 Base de datos

-👉 Descripción de las variables

-🍷 Conclusiones finales

## ¿Cuál es la necesidad o problema a resolver? 

La calidad del vino es influenciada por una variedad de factores, como sus propiedades químicas y características organolépticas. Resolver el desafío de identificar la relación entre estos factores y la calidad del vino nos permitirá no solo comprender mejor los matices que influyen en su sabor y percepción, sino también tener una visión más completa de la complejidad detrás de esta apreciada bebida y la experiencia del consumidor. 

Además, al comparar vinos blancos y tintos en términos de calidad, podemos descubrir patrones específicos asociados con cada tipo y arrojar luz sobre posibles diferencias en sus procesos de elaboración.

## Preguntas:
1. ¿Entre vino blanco y tinto, qué tipo tuvo mejor calificación en calidad?
2. ¿Existe una relación entre cada factor y la calidad del vino?
3. ¿Cuál es la influencia de la concentración de alcohol en la calidad del vino y cómo se compara esta influencia entre vinos blancos y tintos? 

## 📊 Base De Datos:

Fuente: 
[Base en Kaggle](https://www.kaggle.com/datasets/ruthgn/wine-quality-data-set-red-white-wine)

Descripción del dataset:
Este conjunto de datos contiene información de 1599 muestras de vino tinto y 4898 muestras de vino blanco.
Debido a problemas de privacidad y logística, no hay datos sobre los tipos de uva, la marca del vino y el precio de venta del vino.


## Descripción de las variables

Las variables de entrada en el conjunto de datos consisten en el tipo de vino (ya sea vino tinto o vino blanco) y métricas de pruebas objetivas (por ejemplo, niveles de acidez, valores de pH, contenido alcohólico, etc.), mientras que la variable objetivo/salida es una puntuación numérica basada en datos sensoriales, que es la mediana de al menos 3 evaluaciones realizadas por expertos en vinos (En una escala del 0 - muy malo a 10 - excelente).

Para esta consultoría nos enfocaremos en las siguientes 5 variables que comunmente se cree tienen mayor influencia en la calidad percibida del vino:

Tipo de vino: El tipo de vino, ya sea tinto o blanco, es uno de los factores más influyentes, ya que afecta fundamentalmente el perfil de sabor, aroma y estructura del vino.
Acidez fija: La acidez fija es crucial para la frescura y la viveza del vino. Una acidez equilibrada puede realzar los sabores y mantener el vino en equilibrio.
Azúcar residual: El nivel de azúcar residual afecta directamente la percepción de dulzura del vino, lo cual puede tener un impacto importante en cómo se percibe el vino en términos de equilibrio y gusto.
pH: El pH influye en la acidez y la sensación en boca del vino. Un pH adecuado es esencial para mantener la frescura y el equilibrio en el vino.
Alcohol: El contenido de alcohol afecta la sensación en boca, la intensidad de los sabores y la estructura del vino. Un equilibrio adecuado es esencial para lograr una experiencia agradable.
