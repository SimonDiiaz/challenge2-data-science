# 📊 Telecom X - Análisis de Evasión de Clientes

## 🎯 Descripción del Proyecto

Este proyecto forma parte del desafío de análisis de datos para **Telecom X**, donde se analiza el comportamiento de churn (evasión) de clientes para identificar patrones y factores que contribuyen a la cancelación de servicios.

## 🚀 Objetivos

- **Extraer** datos desde una API JSON de manera eficiente
- **Transformar** y limpiar los datos aplicando conceptos de ETL
- **Analizar** patrones de churn mediante EDA (Análisis Exploratorio de Datos)
- **Visualizar** tendencias y correlaciones estratégicas
- **Generar** insights accionables para reducir la evasión de clientes

## 📁 Estructura del Proyecto

```
challenge2-data-science-LATAM/
│
├── TelecomX_Data.json          # Datos fuente en formato JSON
├── TelecomX_diccionario.md     # Diccionario de datos
├── TelecomX_LATAM.ipynb        # Notebook principal con análisis
├── README.md                   # Documentación del proyecto
└── telecom_churn_processed.csv # Dataset procesado (generado)
```

## 🛠️ Tecnologías Utilizadas

- **Python 3.x**
- **Pandas** - Manipulación y análisis de datos
- **NumPy** - Operaciones numéricas
- **Matplotlib** - Visualización de datos
- **Seaborn** - Visualizaciones estadísticas avanzadas
- **Scikit-learn** - Preprocesamiento de datos
- **JSON** - Manejo de datos estructurados

## 📋 Requisitos e Instalación

### Dependencias

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Instalación

1. **Clonar el repositorio:**
```bash
git clone <repository-url>
cd challenge2-data-science-LATAM
```

2. **Instalar dependencias:**
```bash
pip install -r requirements.txt
```

3. **Ejecutar el notebook:**
```bash
jupyter notebook TelecomX_LATAM.ipynb
```

## 🔄 Proceso ETL

### 📌 Extracción
- Carga de datos desde archivo JSON
- Validación de estructura de datos
- Identificación de registros totales

### 🔧 Transformación
- **Aplanamiento** de estructura JSON anidada
- **Limpieza** de datos inconsistentes
- **Conversión** de tipos de datos
- **Creación** de variables derivadas (servicios adicionales)
- **Filtrado** de registros válidos

### 📊 Carga y Análisis
- Análisis exploratorio de datos (EDA)
- Visualizaciones estratégicas
- Análisis de correlaciones
- Identificación de factores de riesgo

## 📈 Principales Hallazgos

### 🚨 Factores de Alto Riesgo de Churn

1. **Método de Pago**: Electronic check presenta mayor tasa de churn
2. **Tipo de Contrato**: Contratos mes a mes tienen mayor riesgo
3. **Servicios de Internet**: Fiber optic muestra mayor evasión
4. **Tenure**: Clientes nuevos (≤12 meses) tienen mayor probabilidad de cancelar

### 📊 Correlaciones Clave

- **Tenure vs Churn**: Correlación negativa fuerte (-0.35)
- **Cargos Mensuales**: Correlación positiva con churn
- **Servicios Adicionales**: Menor churn con más servicios contratados

## 💡 Recomendaciones Estratégicas

### 1. 🎯 Retención Temprana
- Programa de seguimiento intensivo para clientes nuevos
- Incentivos especiales en los primeros 12 meses
- Onboarding mejorado

### 2. 💳 Optimización de Métodos de Pago
- Promover pagos automáticos con descuentos
- Reducir dependencia de cheques electrónicos
- Facilitar cambios de método de pago

### 3. 📝 Estrategia de Contratos
- Incentivar contratos de largo plazo (1-2 años)
- Beneficios exclusivos para contratos extendidos
- Penalizaciones por cancelación temprana

### 4. 🌐 Mejora de Servicios
- Optimizar calidad del servicio Fiber optic
- Crear paquetes atractivos de servicios adicionales
- Soporte técnico proactivo

### 5. 🎯 Segmentación de Clientes
- Perfiles de riesgo basados en variables identificadas
- Estrategias personalizadas por segmento
- Modelos predictivos de churn

## 💰 Impacto Económico

- **Tasa de Churn Actual**: ~26.5%
- **Pérdida Mensual Estimada**: $139,000+
- **Pérdida Anual Estimada**: $1.67M+
- **ROI Potencial**: Reducción del 10% en churn = $167K anuales

## 📊 Visualizaciones Incluidas

1. **Distribución de Churn** - Gráfico circular
2. **Churn por Demografía** - Análisis por género, edad, familia
3. **Análisis de Contratos** - Impacto del tipo de contrato
4. **Distribución de Cargos** - Histogramas y boxplots
5. **Matriz de Correlación** - Heatmap de variables clave
6. **Análisis de Tenure** - Segmentación temporal
7. **Scatter Plots** - Relaciones entre variables numéricas

## 🔍 Análisis de Correlación Extra

Como parte del análisis adicional, se exploró:

- **Correlación entre cargos diarios y evasión**
- **Impacto de la cantidad de servicios contratados**
- **Matrices de correlación con visualización de heatmaps**
- **Gráficos de dispersión para identificar patrones**

## 🚀 Próximos Pasos

1. **Modelado Predictivo**
   - Implementar algoritmos de Machine Learning
   - Validación cruzada y optimización de hiperparámetros
   - Métricas de evaluación (Precision, Recall, F1-Score)

2. **Automatización**
   - Pipeline de datos automatizado
   - Dashboard en tiempo real
   - Alertas automáticas para clientes de alto riesgo

3. **A/B Testing**
   - Probar estrategias de retención
   - Medir impacto de las recomendaciones
   - Optimización continua

## 📝 Uso del Proyecto

### Ejecutar Análisis Completo

```python
# Abrir el notebook
jupyter notebook TelecomX_LATAM.ipynb

# Ejecutar todas las celdas secuencialmente
# Los resultados se guardarán automáticamente
```

### Cargar Datos Procesados

```python
import pandas as pd

# Cargar dataset procesado
df = pd.read_csv('telecom_churn_processed.csv')
print(f"Dataset cargado: {df.shape}")
```

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crear una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abrir un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE.md](LICENSE.md) para detalles.

## 👥 Autor

**Tu Nombre** - Analista de Datos
- LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)
- Email: tu.email@ejemplo.com

## 🙏 Agradecimientos

- Telecom X por proporcionar los datos del desafío
- Comunidad de Data Science LATAM
- Bibliotecas open source utilizadas

---

⭐ **¡Si este proyecto te fue útil, no olvides darle una estrella!** ⭐