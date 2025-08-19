#  Análisis Predictivo de Cancelación de Clientes (Churn)

Este proyecto tiene como objetivo analizar los factores que influyen en la cancelación del servicio por parte de los clientes de una empresa de telecomunicaciones. Se utilizaron técnicas de análisis de datos, ingeniería de características, balanceo de clases y diversos algoritmos de machine learning para predecir y entender el comportamiento de abandono.

---

## 🧾 Estructura del Proyecto

### Carga y Limpieza de Datos
- Dataset: 7.032 registros de clientes con múltiples variables categóricas y numéricas.
- Se eliminaron columnas irrelevantes y se transformaron variables categóricas con `OneHotEncoder`.

### Preprocesamiento
- Aplicación de `LabelEncoder` a la variable objetivo (`cancelado`).
- Estandarización mediante `MinMaxScaler` para algoritmos sensibles a la escala.
- Balanceo de clases con `NearMiss (version=3)` para corregir el desbalance de clases (mayoría de clientes que no cancelan).

### Modelado Predictivo
Se compararon diferentes modelos:
- **Árbol de Decisión**
- **Random Forest**
- **K-Nearest Neighbors (KNN)** con y sin normalización
- **Regresión Logística**

### Evaluación de Modelos
Se utilizaron métricas como:
- **Accuracy**
- **Precision**
- **Recall** (enfocado en detectar clientes que cancelan)


## 📈 Visualizaciones

- Matriz de correlación
- Boxplots de cancelación vs meses contratados y gastos totales
- Gráficos de importancia de variables (barplots)

---

## 🧠 Tecnologías Utilizadas

- Python 
- Pandas, NumPy, Matplotlib, Seaborn, Plotly
- Scikit-learn
- Imbalanced-learn 
- Modelos: `DecisionTreeClassifier`, `RandomForestClassifier`, `KNeighborsClassifier`, `LogisticRegression`


## ✅ Conclusiones

- El factor más crítico es la antigüedad del cliente.
- Contratos de corto plazo, pagos no automáticos y altos costos iniciales están fuertemente asociados con la cancelación.
- Las variables demográficas también influyen, pero en menor medida.


## 📌 Recomendaciones Estratégicas

- Incentivar contratos anuales o bianuales.
- Implementar descuentos y beneficios para pagos automáticos.
- Monitorear la experiencia de clientes nuevos y ofrecer soporte personalizado en los primeros meses.
- Revisar percepción de valor en segmentos con gastos elevados.


## 📝 Licencia

MIT - Uso libre para fines educativos y no comerciales.
