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

## Paso 2: Ingeniería de Características o Datos
Crea nuevas características, categoriza y agrupa los datos para mejorar la precisión del modelo de Machine Learning en Azure.

## Paso 3: Análisis Exploratorio
Realiza un análisis visual y estadístico para comprender los datos, identificar patrones y detectar anomalías.

## Paso 4: Balanceo de Clases y Preparación de los Archivos para el Modelo
Aplica SMOTE para balancear las clases y utiliza train_test_split() para preparar conjuntos de datos de entrenamiento y prueba.

## Paso 5: Entrenamiento y Despliegue del Modelo de Clasificación ML
Entrena el modelo de clasificación y despliega el modelo en Azure para su uso en producción.
