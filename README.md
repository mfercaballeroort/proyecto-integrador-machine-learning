# Proyecto Integrador - Machine Learning

## Titanic: preparación y análisis para aprendizaje supervisado

Este proyecto forma parte de una práctica de aprendizaje automático supervisado. Se utiliza el dataset del Titanic para realizar un proceso completo de exploración y preparación de datos antes de aplicar modelos de Machine Learning.

## Objetivo

Preparar un dataset adecuado para un problema de clasificación binaria, identificando y tratando los valores faltantes, transformando las variables categóricas, seleccionando las variables predictoras y realizando un análisis exploratorio de los datos.

## Dataset

El dataset utilizado corresponde a información de pasajeros del Titanic.

La variable objetivo es:

- `Survived`: indica si el pasajero sobrevivió (1) o no sobrevivió (0).

Entre las variables analizadas se encuentran:

- `Pclass`: clase del pasajero
- `Sex`: sexo
- `Age`: edad
- `SibSp`: cantidad de hermanos o cónyuges a bordo
- `Parch`: cantidad de padres o hijos a bordo
- `Fare`: tarifa abonada
- `Embarked`: puerto de embarque

## Proceso realizado

El proyecto incluye las siguientes etapas:

1. Carga y exploración inicial del dataset.
2. Análisis de tipos de variables.
3. Análisis exploratorio de datos (EDA).
4. Identificación y tratamiento de valores faltantes.
5. Detección de registros duplicados.
6. Análisis de valores atípicos.
7. Análisis de correlaciones.
8. Selección de variables predictoras.
9. División del dataset en conjuntos de entrenamiento y prueba.
10. Imputación de valores faltantes.
11. Transformación de variables categóricas mediante One-Hot Encoding.
12. Estandarización de variables numéricas mediante StandardScaler.
13. Preparación del dataset para el modelado.

## Selección de variables

Se excluyeron las variables `PassengerId`, `Name`, `Ticket` y `Cabin`.

Se conservaron `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare` y `Embarked` debido a su posible utilidad para explicar y predecir la supervivencia.

## Tratamiento de datos

Los valores faltantes de `Age` fueron imputados utilizando la mediana calculada sobre el conjunto de entrenamiento.

Los valores faltantes de `Embarked` fueron tratados utilizando la categoría más frecuente del conjunto de entrenamiento.

Las variables categóricas `Sex` y `Embarked` fueron transformadas mediante One-Hot Encoding.

Las variables numéricas fueron estandarizadas mediante `StandardScaler`.

## Tipo de problema

**Aprendizaje supervisado - Clasificación binaria**

La variable objetivo es `Survived`, que representa si el pasajero sobrevivió o no.

## Herramientas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub

## Resultado

Al finalizar esta etapa, el dataset queda preparado para la siguiente fase del proyecto: el entrenamiento y evaluación de diferentes modelos de clasificación.

En esta Pre-Entrega no se realiza entrenamiento ni evaluación de modelos.

## Notebook

El análisis completo se encuentra en:

**`Proyecto_Integrador_Pre-Entrega.ipynb`**

---

### Autora

**María Fernanda Caballero**
