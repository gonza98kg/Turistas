# Análisis Exploratorio: Turistas y PST en Hidalgo

**Unidad de Planeación y Prospectiva · Gobierno del Estado de Hidalgo · 2026**

---

## ¿Qué es este proyecto?

Se recibió la base de datos resultante de un instrumento de levantamiento de información aplicado en tres destinos turísticos del Estado de Hidalgo. El análisis exploratorio de los datos tuvo como objetivo identificar el perfil de los visitantes y los Prestadores de Servicios Turísticos (PST), con la finalidad de proveer insumos para el desarrollo de una **aplicación oficial de turismo estatal**.

Los hallazgos e insights derivados fueron entregados al equipo de desarrollo para la definición de los MVP de la aplicación.

---

## Datos

| Población | Muestra |
|---|---|
| Turistas | 807 encuestas |
| Prestadores de Servicios Turísticos (PST) | ~100 encuestas |

---

## Preguntas que guiaron el análisis

**Turistas**
- ¿De dónde provienen? ¿Cómo y cuándo viajan?
- ¿Qué los motiva a visitar Hidalgo?
- ¿Qué canales usan para buscar inspiración?
- ¿Qué esperan de una app de turismo del gobierno estatal?

**PST**
- ¿Cuál es su perfil y tipo de servicio?
- ¿Qué canales de promoción utilizan actualmente?
- ¿Qué barreras de crecimiento enfrentan?
- ¿Qué tan abiertos están a adoptar una plataforma digital?

---

## Metodología

### Turistas
La base llegó en condiciones relativamente limpias. Se eliminaron columnas duplicadas con valores nulos, se estandarizaron las columnas geográficas para su lectura en Looker Studio, se recodificaron respuestas mixtas (texto libre y escala numérica) en la variable de intención de uso de la app, y se agruparon los canales de inspiración en categorías comparables.

### PST
Requirió un tratamiento más profundo dado que la mayoría de las variables eran respuestas abiertas. Se aplicó categorización semántica para convertir texto libre en variables analíticas estructuradas: tipo de servicio, canales de promoción, estacionalidad, barreras de crecimiento, percepción tecnológica, confianza digital y motivadores de retención. Este proceso permitió cuantificar dimensiones cualitativas que de otro modo no serían representables en un dashboard.

Los datos procesados de ambas poblaciones se exportan como archivos `.csv` para su visualización en **Looker Studio**.

---

## Hallazgos principales

- El grueso de los visitantes proviene de **Hidalgo, Estado de México y CDMX**, con un perfil predominantemente joven (18–39 años) y distribución equitativa por género.
- El **55% viaja varias veces al año** dentro de México, lo que indica un segmento de viajeros frecuentes con alto potencial de fidelización.
- El **64.6% de los PST no utiliza ninguna app o plataforma digital** para promocionarse, validando la pertinencia de la iniciativa estatal.
- La **estacionalidad** afecta al 54.5% de los PST, con impacto predominantemente negativo — señal de oportunidad para una plataforma que distribuya la demanda.
- En ambas poblaciones, la adopción tecnológica está condicionada por **resultados tangibles**: los turistas priorizan personalización y facilidad de uso; los PST, incremento directo en ventas y visibilidad.

---

## Estructura del repositorio

| Archivo | Descripción |
|---|---|
| `code.ipynb` | Notebook con EDA, limpieza y exportación de ambas bases |
| `TURISTAS_data.csv` | Base de datos original — turistas |
| `PST_data.csv` | Base de datos original — PST |
| `Insights_Turistas.pdf` | Reporte de hallazgos — turistas |
| `Insights_Prestadores.pdf` | Reporte de hallazgos — PST |

---

## Tecnologías

`Python` · `pandas` · `numpy` · `Looker Studio`
