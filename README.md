# Comparador de Sistemas Previsionales (CJPPU - Uruguay)

## Objetivo del Proyecto
El objetivo de este proyecto es proporcionar una herramienta visual e interactiva para profesionales universitarios en Uruguay que permita comparar dos regímenes de aportación distintos (10 categorías vs. 15 categorías) dentro de la **CJPPU (Caja de Jubilaciones y Pensiones de Profesionales Universitarios)**. La herramienta facilita la comprensión del impacto financiero de las decisiones de aportación a lo largo del tiempo, calculando tanto la inversión total requerida como el haber jubilatorio mensual estimado.

## Premisas y Lógica de Cálculo
Este simulador permite proyectar escenarios jubilatorios dinámicos basados en la normativa vigente:
*   **Edad Jubilatoria:** Configurable mediante el selector (60 a 70+ años).
*   **Tasa de Adquisición de Derechos (TAD):** El porcentaje aplicado por cada año de servicio varía según la edad de retiro seleccionada (ej. 1.20% a los 60 años, 1.50% a los 65 años, hasta 1.96% a los 70+ años).
*   **Cálculo del Haber:** Se obtiene multiplicando la **TAD** correspondiente a la edad por la **Sumatoria de Años de Servicio** totales. Este porcentaje se aplica sobre el promedio de los mejores 240 meses (20 años) de sueldos fictos de aportación.

## Fuente de Datos
Los valores de sueldos fictos y alícuotas de aportación utilizados en este simulador fueron extraídos de la documentación oficial de la CJPPU:
*   **Fuente:** [CJPPU - Escalas de Sueldos Fictos y Aportes](https://www.cjppu.org.uy/download.php?m=acts&i=106)
*   **Fecha de Acceso:** 7 de abril de 2026.

## Guía de Uso del Simulador

### 1. Edad de Jubilación y TAD
Seleccione la **Edad de Jubilación** deseada. El sistema asignará automáticamente la **Tasa de Adquisición de Derechos (TAD)** correspondiente. Podrá visualizar los **Años Totales** calculados para cada sistema al lado del selector, facilitando el control de la meta de años de aporte.

### 2. Configuración del Historial Base
Ingrese la cantidad de años ya aportados en cada categoría en la sección **"Historial Base"**. Estos años se consideran servicios ya cumplidos y se aplicarán de forma idéntica a ambos sistemas comparados. Dispones de un botón **Reset** exclusivo para esta sección.

### 3. Simulación de Aportación Futura
En las tablas de **Sistema 10** y **Sistema 15**, ingrese la proyección de años que planea aportar en cada categoría hacia el futuro.
*   Utilice los botones de **Reset** en cada sección para limpiar los valores y reiniciar la simulación.

### 4. Interpretación de Resultados (Dashboard)
El **Dashboard Comparativo** se actualiza en tiempo real:
*   **Jubilación Estimada:** El haber mensual nominal que percibiría al momento del retiro.
*   **Inversión Total:** La sumatoria nominal de todos los aportes mensuales realizados durante la carrera profesional.
*   **Diferencia de Inversión:** Indica qué sistema representa una mayor carga contributiva y en qué cuantía.
*   **Tiempo de Recuperación (Punto de Equilibrio):** Calcula cuántos años de percepción del mayor haber jubilatorio son necesarios para amortizar el excedente de capital invertido en aportes.

## Próximas Etapas (Next Steps)
Este proyecto se encuentra en fase de desarrollo activo y continuará iterando. Las futuras actualizaciones incluirán:
*   **Causales Jubilatorias Adicionales:** Implementación de variables para escenarios de invalidez o regímenes especiales.
*   **Ajustes por Inflación/Unidades:** Opciones para simular proyecciones basadas en ajustes de unidades de cuenta o proyecciones de IPC.

---
*Descargo de responsabilidad: Esta herramienta tiene fines informativos y de simulación únicamente. Los cálculos jubilatorios oficiales deben ser validados directamente ante la CJPPU.*
