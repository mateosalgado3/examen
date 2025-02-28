Descripción
Este proyecto analiza los datos de consumo de clientes de la empresa Megaline para:

Predecir el consumo futuro (minutos, SMS y megabytes) basado en el historial.
Estimar el costo total esperado de cada usuario en el siguiente mes.
Optimizar estrategias de negocio con base en los patrones de consumo.
El análisis sigue una estructura organizada en seis fases, documentadas en Jupyter Notebooks.

📌 Requisitos del Proyecto
Antes de ejecutar el proyecto, asegúrate de tener instalado Python 3.8+ y las siguientes librerías:

bash
Copiar
Editar
pip install -r requirements.txt
Si deseas instalar solo las principales dependencias, usa:

bash
Copiar
Editar
pip install pandas numpy scikit-learn matplotlib seaborn joblib statsmodels
📌 Estructura del Proyecto
📁 Proyecto_Megaline/
│── 📂 data/raw/ → Datos originales (CSV sin procesar).
│── 📂 data/clean/ → Datos limpios y modelados (listos para análisis).
│── 📂 data/ml/ → Dataset final con Feature Engineering.
│── 📂 notebooks/ → Contiene los notebooks de cada fase.
│── 📂 models/ → Modelos entrenados guardados.
│── 📄 requirements.txt → Librerías necesarias.
│── 📄 README.md → Este archivo.

📌 Pasos para Reproducir el Proyecto
Sigue estos pasos en WSL o cualquier entorno compatible:

1️⃣ Clonar o Descargar el Proyecto
Si tienes acceso a un repositorio, clónalo con:

bash
Copiar
Editar
git clone [URL_DEL_REPO]
cd Proyecto_Megaline
Si descargaste el ZIP, descomprime el proyecto en una carpeta de trabajo.

2️⃣ Verificar las Librerías
Ejecuta:

bash
Copiar
Editar
pip list
Si faltan librerías, instálalas con:

bash
Copiar
Editar
pip install -r requirements.txt
3️⃣ Ejecutar el Proyecto Paso a Paso
Ejecuta cada Jupyter Notebook en orden:

📌 Ejecutar Jupyter Notebook:

bash
Copiar
Editar
jupyter notebook
📂 Notebooks a Ejecutar:
1️⃣ 1_EDA.ipynb – Exploración de datos (estadísticas, visualizaciones, valores atípicos).
2️⃣ 2_Data_Wrangling.ipynb – Limpieza, manejo de valores nulos y unificación de datasets.
3️⃣ 3_Modeling.ipynb – Modelado de datos (Star Schema).
4️⃣ 4_Feature_Engineering.ipynb – Creación de variables nuevas y escalado.
5️⃣ 5_ML_Training.ipynb – Entrenamiento de modelos de Machine Learning.
6️⃣ 6_Conclusions.ipynb – Conclusiones y recomendaciones de negocio.

4️⃣ Ver Resultados
📌 📂 Datos generados:

data/clean/ → Datos limpios y modelados.
data/ml/ → Dataset final con Feature Engineering.
models/ → Modelos entrenados guardados con joblib.
📌 📂 Modelos entrenados:
Los modelos están guardados en models/ y se pueden cargar así:

python
Copiar
Editar
import joblib
modelo = joblib.load("models/mejor_modelo.pkl")
📌 📂 Métricas de los modelos:
Las métricas (RMSE, MAE, R²) están documentadas en 5_ML_Training.ipynb.

📌 Recomendaciones Finales
✅ Si hay errores al ejecutar, verifica que todas las rutas de archivos sean correctas.
✅ Si falta alguna librería, usa pip install [librería] para instalarla manualmente.