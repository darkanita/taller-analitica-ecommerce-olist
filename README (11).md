# 🛒 Taller de Analítica de Datos - Caso Olist E-commerce

## 📋 Descripción

Este taller utiliza datos reales del **marketplace brasileño Olist** para practicar SQL y Python en un contexto de negocio realista. Los estudiantes asumirán el rol de Analistas de Datos que deben responder preguntas estratégicas del equipo de negocio.

## 📊 Dataset

**Brazilian E-Commerce Public Dataset by Olist**
- Fuente: [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- Periodo: 2016-2018
- Registros: ~100,000 pedidos
- Tablas: 9 tablas relacionales

### Estructura del Dataset

```
customers ─────┐
               │
orders ────────┼──── order_items ──── products
               │          │
               │          └──── sellers
               │
order_payments │
               │
order_reviews ─┘
```

## 📁 Estructura del Taller

```
taller_olist/
├── README.md                              # Este archivo
├── 01_Taller_SQL_Olist.ipynb             # Taller de SQL (Básico → Intermedio)
├── 02_Taller_Python_Preprocesamiento.ipynb # Taller de Python/Pandas
├── 03_Taller_Integrador_SQL_Python.ipynb  # Proyecto final integrador
└── data/                                  # Carpeta para los CSVs (crear)
```

## 🚀 Instrucciones de Configuración

### Paso 1: Descargar el Dataset

**Opción A - Desde Kaggle (recomendado):**
1. Crear cuenta en [Kaggle](https://www.kaggle.com/)
2. Ir a Account → Create New API Token
3. Guardar `kaggle.json` en `~/.kaggle/`
4. Ejecutar en terminal:
```bash
pip install kaggle
kaggle datasets download -d olistbr/brazilian-ecommerce --unzip -p ./data/
```

**Opción B - Descarga manual:**
1. Ir a [https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
2. Click en "Download"
3. Descomprimir en la carpeta `./data/`

### Paso 2: Instalar Dependencias

```bash
pip install pandas numpy matplotlib seaborn sqlalchemy jupyter ipython-sql
```

### Paso 3: Crear la Base de Datos

Ejecutar las primeras celdas del notebook `01_Taller_SQL_Olist.ipynb` para crear `olist.db`.

## 📚 Contenido de los Talleres

### Taller 1: SQL (01_Taller_SQL_Olist.ipynb)

| Parte | Tema | Dificultad |
|-------|------|------------|
| 1 | SELECT, WHERE, ORDER BY | ⭐⭐ |
| 2 | COUNT, SUM, AVG, GROUP BY | ⭐⭐⭐ |
| 3 | JOINs - Conectando tablas | ⭐⭐⭐⭐ |
| 4 | Subconsultas y análisis avanzado | ⭐⭐⭐⭐ |
| Final | Reporte Ejecutivo | ⭐⭐⭐⭐⭐ |

### Taller 2: Python/Preprocesamiento (02_Taller_Python_Preprocesamiento.ipynb)

| Parte | Tema | Dificultad |
|-------|------|------------|
| 1 | Exploración con Pandas | ⭐⭐ |
| 2 | Manejo de valores nulos | ⭐⭐⭐ |
| 3 | Detección de outliers | ⭐⭐⭐ |
| 4 | Transformación de datos | ⭐⭐⭐⭐ |
| 5 | Integración (merge) | ⭐⭐⭐⭐ |
| Final | Dataset analítico limpio | ⭐⭐⭐⭐⭐ |

### Taller 3: Integrador (03_Taller_Integrador_SQL_Python.ipynb)

| Métrica | Habilidades |
|---------|------------|
| Evolución de ventas | SQL + Visualización |
| Top categorías | SQL + Gráficos de barras |
| Distribución geográfica | SQL + Gráficos circulares |
| Satisfacción del cliente | SQL + Análisis cruzado |
| Rendimiento de entregas | SQL + Series temporales |

## 🎯 Preguntas de Negocio que Responde el Taller

1. ¿Cuál es el total de ingresos por mes?
2. ¿Cuáles son las categorías más vendidas?
3. ¿De qué estados provienen la mayoría de los clientes?
4. ¿Cuál es la calificación promedio de satisfacción?
5. ¿Qué porcentaje de entregas son tardías?
6. ¿Cómo se relaciona el tiempo de entrega con la satisfacción?
7. ¿Quiénes son los vendedores más exitosos?
8. ¿Qué método de pago prefieren los clientes?

## 💡 Tips para Instructores

1. **Progresión gradual:** SQL es más fácil, comenzar ahí genera confianza
2. **Contexto de negocio:** Cada ejercicio tiene una "pregunta de negocio" real
3. **Soluciones ocultas:** Usar `<details>` para que los estudiantes intenten primero
4. **Desafíos finales:** Cada taller termina con un proyecto integrador

## 📖 Recursos Adicionales

- [Documentación de Pandas](https://pandas.pydata.org/docs/)
- [Tutorial de SQL](https://www.w3schools.com/sql/)
- [Visualización con Matplotlib](https://matplotlib.org/stable/gallery/index.html)
- [Dataset original en Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## ✅ Checklist Pre-Clase

- [ ] Dataset descargado y descomprimido en `./data/`
- [ ] Dependencias instaladas
- [ ] Base de datos SQLite creada (`olist.db`)
- [ ] Notebooks ejecutados sin errores
- [ ] Proyector/pantalla configurado para mostrar notebooks

---

**¡Éxito con tu clase! 🚀**
