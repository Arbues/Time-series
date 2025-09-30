# Time-series
It encompasses topics related to time series


## 📋 **Resumen del Curso: Manejo de Series Temporales con Modelos Básicos en Python**

### **🎯 Objetivo General**
Introducir los fundamentos del análisis y modelado de series temporales, desde la descomposición básica hasta predicciones utilizando modelos clásicos.

---

## **📊 Módulos del Curso**

### **1. 🏗️ Fundamentos de Series de Tiempo**

**Conceptos Clave:**
- ✅ **Definición**: Secuencias de datos ordenados en el tiempo
- ✅ **Componentes Esenciales**:
  - Tendencia (movimiento a largo plazo)
  - Estacionalidad (patrones que se repiten)
  - Ciclo (fluctuaciones no periódicas)
  - Ruido (variabilidad aleatoria)

**Herramientas Implementadas:**
- ✅ **Pandas** para manipulación de datos temporales
- ✅ **Matplotlib** para visualización
- ✅ **Statsmodels** para análisis estadístico

---

### **2. 🔍 Descomposición de Series Temporales**

**Dos Enfoques Principales:**

#### **📈 Modelo ADITIVO**
- ✅ **Fórmula**: `Serie = Tendencia + Estacionalidad + Ruido`
- ✅ **Caso de Uso**: Cuando la estacionalidad es constante en el tiempo
- ✅ **Aplicación Práctica**: Ventas de bebidas mensuales

```python
# Implementación
result_aditivo = seasonal_decompose(serie, model='additive')
```

#### **📊 Modelo MULTIPLICATIVO**
- ✅ **Fórmula**: `Serie = Tendencia × Estacionalidad × Ruido`
- ✅ **Caso de Uso**: Cuando la variabilidad crece con la tendencia
- ✅ **Aplicación Práctica**: Precios del petróleo (varianza cambiante)

```python
# Implementación
result_mult = seasonal_decompose(serie, model='multiplicative')
```

---

### **3. 🔮 Técnicas de Predicción**

**Metodología Implementada:**

#### **Predicción por Componentes**
1. ✅ **Tendencia**: Modelo de regresión lineal
2. ✅ **Estacionalidad**: Repetición del patrón histórico
3. ✅ **Combinación**: Suma (aditivo) o multiplicación (multiplicativo)

#### **Transformación Logarítmica**
- ✅ **Propósito**: Convertir modelo multiplicativo a aditivo
- ✅ **Beneficio**: Estabilizar la varianza
- ✅ **Fórmula**: `log(Serie) = log(Tendencia) + log(Estacionalidad)`

```python
# Transformación y predicción
trend_log = np.log(tendencia)
predicción = exp(tendencia_predicha) * exp(estacionalidad_predicha)
```

---

### **4. 🛠️ Casos Prácticos Implementados**

#### **Caso 1: Ventas de Bebidas (Aditivo)**
- ✅ 36 meses de datos históricos
- ✅ Patrón estacional claro
- ✅ Predicción de 24 meses futuros

#### **Caso 2: Precios del Petróleo (Multiplicativo)**
- ✅ 352 observaciones mensuales (1990-2019)
- ✅ Tendencia creciente con varianza variable
- ✅ Manejo de datos con decimales y formatos

---

### **5. 📈 Metodología de Trabajo**

**Flujo de Análisis:**
1. ✅ **Carga y limpieza** de datos temporales
2. ✅ **Exploración visual** con gráficos de series
3. ✅ **Selección del modelo** (aditivo vs multiplicativo)
4. ✅ **Descomposición** en componentes
5. ✅ **Predicción individual** por componente
6. ✅ **Combinación** de predicciones
7. ✅ **Validación** visual de resultados

---

### **6. 🎯 Habilidades Desarrolladas**

**Técnicas:**
- ✅ Manipulación de índices temporales en Pandas
- ✅ Identificación visual de patrones estacionales
- ✅ Aplicación correcta de modelos aditivos vs multiplicativos
- ✅ Implementación de regresión lineal para tendencias
- ✅ Transformaciones logarítmicas para estabilización

**Analíticas:**
- ✅ Capacidad para reconocer estacionariedad
- ✅ Comprensión de varianza constante vs variable
- ✅ Habilidad para seleccionar el modelo apropiado
- ✅ Capacidad de realizar predicciones básicas

---

### **7. 🔄 Proyección a Temas Avanzados**

**Base para:**
- ✅ **Modelos ARIMA** y **SARIMA**
- ✅ **Pruebas de estacionariedad** (Dickey-Fuller, KPSS)
- ✅ **Modelos de suavizado exponencial**
- ✅ **Series multivariadas** y **cointegración**
- ✅ **Redes neuronales** para series temporales (LSTM)

---

## **📚 Valor del Curso**

**Para la Agrupación:**
- ✅ **Fundamentos sólidos** en análisis temporal
- ✅ **Herramientas prácticas** inmediatamente aplicables
- ✅ **Comprensión intuitiva** de conceptos estadísticos
- ✅ **Base matemática** para modelos avanzados
- ✅ **Capacidad de toma de decisiones** basada en patrones temporales

---

## **🚀 Próximos Pasos Sugeridos**

**Temas para profundizar:**
- Modelos ARIMA/SARIMA para series estacionarias
- Pruebas de raíz unitaria y diferenciación
- Métricas de error en predicciones (MAE, RMSE, MAPE)
- Modelos de suavizado exponencial (Holt-Winters)
- Aplicaciones en finanzas, economía y negocios

---

