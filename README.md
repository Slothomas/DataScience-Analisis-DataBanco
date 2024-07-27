### Tecnologias Utilizadas

<p align="center">
    <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/jupyernotebook-coolab.png" alt="Google Colab, Jupyter Notebook" width="250" height="120"/>
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/azure-ml.jpg" alt="Azure Machine Learning" width="250" height="120"/>
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/python-pandas.png" alt="Pandas, Python" width="250" height="120"/>
</p>

# DataScience-Analisis-DataBanco
Analisis de datos de un banco para limpieza de datos, aplicar ingeneria de datos y construir modelo Machine Learning en la nube Azure

## Descripción del Problema de Negocio

En el sector bancario, la identificación precisa del propósito de las solicitudes de crédito es crucial para ofrecer productos financieros adecuados y estrategias de marketing personalizadas. Las instituciones financieras enfrentan el desafío de segmentar a sus clientes de manera efectiva para maximizar el impacto de sus ofertas y mejorar la satisfacción del cliente.

## Problema:

Las entidades bancarias a menudo tienen dificultades para comprender las intenciones exactas detrás de las solicitudes de crédito de sus clientes debido a la falta de datos estructurados y la presencia de información no estandarizada. Esto puede llevar a una asignación ineficiente de recursos, ofertas de productos que no se alinean con las necesidades del cliente y, en última instancia, una pérdida de oportunidades de negocio.

## Impacto:

- Ineficiencia en las Campañas de Marketing: Las ofertas de crédito mal dirigidas pueden resultar en bajas tasas de conversión y costos de - adquisición elevados.
- Satisfacción del Cliente: La falta de ofertas relevantes puede disminuir la satisfacción del cliente y la lealtad hacia la institución financiera.
- Oportunidades Perdidas: No identificar correctamente el propósito de las solicitudes puede llevar a la pérdida de oportunidades para ofrecer productos financieros adecuados que se alineen con las necesidades del cliente.

## Solución Propuesta:

Implementar un modelo de Machine Learning para predecir el propósito de las solicitudes de crédito basándose en datos históricos de clientes. Este modelo ayudará a:

- Segmentar Efectivamente a los Clientes: Al identificar patrones y propósitos específicos, se podrán diseñar campañas de marketing más efectivas y dirigidas.
- Optimizar Ofertas de Productos: Ajustar las ofertas de crédito según las necesidades y propósitos identificados, mejorando así la relevancia y el impacto de las ofertas.
- Mejorar la Experiencia del Cliente: Ofrecer productos y servicios que se alineen mejor con las intenciones y necesidades de los clientes, aumentando su satisfacción y lealtad.
- El enfoque en la predicción precisa del propósito de las solicitudes permitirá una toma de decisiones más informada, una asignación de recursos más eficiente y una mejora general en la experiencia del cliente.






## Paso 1: ETL
Carga, estandariza y limpia los datos, convirtiéndolos a un formato numérico adecuado para su procesamiento en Azure.

> <a href="https://colab.research.google.com/drive/1BIE0tmq9tkw9slaO_eUOE0fP_0CObn0T#scrollTo=_PVF66liu2Ur&uniqifier=1" target="_blank">Paso 1</a>

## Paso 2: Ingeniería de Características
Crea nuevas características, categoriza y agrupa los datos para mejorar la precisión del modelo de Machine Learning en Azure.

> <a href="https://colab.research.google.com/drive/1BIE0tmq9tkw9slaO_eUOE0fP_0CObn0T#scrollTo=e620Nyvyv0Lu&uniqifier=1" target="_blank">Paso 2</a>

## Paso 3: Análisis Exploratorio
Realiza un análisis visual y estadístico para comprender los datos, identificar patrones y detectar anomalías.

> <a href="https://colab.research.google.com/drive/1BIE0tmq9tkw9slaO_eUOE0fP_0CObn0T#scrollTo=yg2VujLiwNw6&uniqifier=1" target="_blank">Paso 3</a>

## Paso 4: Balanceo de Clases y Preparación de los Archivos para el Modelo
Aplica SMOTE para balancear las clases y utiliza train_test_split() para preparar conjuntos de datos de entrenamiento y prueba.

> <a href="https://colab.research.google.com/drive/1BIE0tmq9tkw9slaO_eUOE0fP_0CObn0T#scrollTo=skSGVsw0wRqf&uniqifier=1" target="_blank">Paso 4</a>

## Paso 5: Entrenamiento y Despliegue del Modelo de Clasificación ML
Entrena el modelo de clasificación y despliega el modelo en Azure para su uso en producción.

> <a href="https://colab.research.google.com/drive/1BIE0tmq9tkw9slaO_eUOE0fP_0CObn0T#scrollTo=uX_xdGTAwZxC&uniqifier=1" target="_blank">Paso 5</a>

#### - Modelo 1:
En este modelo, se utilizó el archivo 'german_credit_procesadov1.csv' sin aplicar ingeniería de características. Se empleó un modelo de machine learning de clasificación con validación cruzada de k iteraciones y 7 validaciones cruzadas durante una hora. El mejor resultado obtenido fue un Accuracy de 0.3539489, indicando un margen significativo para mejorar.

<p align="center">
    <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo1resultados.png" alt="Resultados Generales" width="905"/>
    </p>
<p align="center">
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo1resultados-matrix.png" alt="Matriz de Confusión" width="450" height="300"/>
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo1resultados-recallpng.png" alt="Precisión y Recall" width="450" height="300"/>
</p>

#### - Modelo 2:
Para este modelo, se utilizó el archivo 'german_credit_procesadov2.csv', que incluye la ingeniería de características del paso 2 y el balanceo de clases del paso 4. Se empleó un modelo de machine learning de clasificación con validación cruzada de k iteraciones y 8 validaciones cruzadas, una más que el modelo anterior, también durante una hora. El mejor resultado obtenido fue un Accuracy de 0.7346501, lo cual representa una mejora significativa, duplicando el indicador y resultando en un modelo más confiable y preciso.

<p align="center">
    <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo2resultados.png" alt="Resultados Generales" width="905"/>
</p>
<p align="center">
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo2resultados-matrix.png" alt="Matriz de Confusión" width="450" height="300"/>
  <img src="https://github.com/Slothomas/DataScience-Analisis-DataBanco/blob/main/img/modelo2resultados-recallpng.png" alt="Precisión y Recall" width="450" height="300"/>
</p>

## ¿Qué queda por delante?
Para avanzar, se deben considerar los siguientes pasos: obtener una base de datos más grande para mejorar el entrenamiento del modelo, aplicar una ingeniería de características más profunda, seguir experimentando con diferentes modelos, y generar filtros más específicos en las categorías. Estos esfuerzos tienen como objetivo incrementar el KPI de **accuracy** y lograr un modelo más preciso y confiable.
