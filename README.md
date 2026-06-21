<div align="center">

# Búsqueda de Raíces Reales — Métodos Numéricos Iterativos

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Numerical](https://img.shields.io/badge/Métodos-Numéricos-FF6B35?style=for-the-badge)
![Math](https://img.shields.io/badge/Newton--Raphson-Convergencia-8E24AA?style=for-the-badge)

> Búsqueda de raíces de funciones reales con el método de Newton-Raphson: análisis de convergencia y criterios de parada.

## Descripción

</div>

---

Implementación y análisis del **método de Newton-Raphson** para búsqueda de raíces reales. Se estudia la convergencia cuadrática del método, se implementan criterios de parada por error relativo y se comparan las tasas de convergencia para diferentes funciones y puntos de partida iniciales.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `convergencia_newton.png` | Gráfica de convergencia del método |
| `Tabla en Excel.xlsx` | Tablas de iteraciones y errores |
| `*.pdf` | Informe con análisis matemático |

## Arquitectura

```mermaid
flowchart TD
    A[newton.py / newton_py.ipynb] --> B[definir f-x y f_prima-x]
    B --> C{criterio_parada - error_relativo}
    C -->|No converge| D[x_n+1 = x_n - f-x_n / f_prima-x_n]
    D --> C
    C -->|Converge| E[guardar_iteraciones]
    E --> F[(resultados_newton_raphson.csv)]
    E --> G[(resultados_newton_sistema.csv)]
    F --> H[convergencia_newton.png - matplotlib]
    G --> H
    H --> I[Analisis de convergencia cuadratica]
```

## Formula de Newton-Raphson

La iteración se define como: **x_{n+1} = x_n - f(x_n) / f_prima(x_n)**

La convergencia es de orden cuadrático cuando la derivada en la raíz es distinta de cero. El criterio de parada es el error relativo entre iteraciones consecutivas.

## Contexto académico

**Asignatura:** Métodos Numéricos · **Institución:** Ingeniería Informática
**Autor:** Alejandro De Mendoza — Ingeniero Informático · Especialista Ingeniería de Software

---

## Autor

**Alejandro De Mendoza**  
Ingeniero Informático · Especialista en IA · Especialista en Ingeniería de Software · Máster en Arquitectura de Software

[![GitHub](https://img.shields.io/badge/GitHub-AlejoTechEngineer-181717?style=for-the-badge&logo=github)](https://github.com/AlejoTechEngineer)
