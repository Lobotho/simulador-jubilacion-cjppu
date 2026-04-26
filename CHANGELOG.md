# Changelog - Comparador de Sistemas Previsionales (CJPPU)

## [7 de Abril de 2026]
### Funcionalidades Iniciales
- **Desarrollo Inicial**: Creación del simulador interactivo para la comparación entre el Sistema de 10 categorías (Art. 59 Inc. 1) y el Sistema de 15 categorías (Art. 59 Inc. 2).
- **Tablas de Proyección**: Implementación de tablas dinámicas que permiten ingresar años de aporte futuros por categoría.
- **Cálculo de Jubilación**: Lógica de cálculo basada en el haber jubilatorio estándar (65 años de edad / 35 años de servicio) con una tasa de reemplazo del 52.5%.
- **Dashboard Comparativo**: Visualización en tiempo real de Jubilación Estimada, Inversión Total, Diferencia de Costo y Tiempo de Recuperación (Breakeven).
- **Exportación a PDF**: Funcionalidad de descarga de reporte optimizada para formato horizontal (Landscape) con dimensiones personalizadas.
- **Botones de Reset**: Incorporación de controles para reiniciar valores en las tablas de Sistema 10 y Sistema 15 de forma independiente.
- **Documentación**: Creación y traducción técnica del `README.md` en español e inglés.

## [25 de Abril de 2026]
### Nuevas Funcionalidades
- **Reinicio de Historial Base**: Adición de un botón de "Reset" específico para la sección de Historial Base, permitiendo limpiar el historial histórico global en un solo clic.
- **Cálculo Dinámico por Edad**: Migración del sistema de cálculo estático (52.5%) a un sistema de cálculo dinámico que depende de la Edad de Jubilación.
- **Diccionario de TAD**: Implementación de una tabla técnica de **Tasa de Adquisición de Derechos (TAD)** que asigna el porcentaje correspondiente desde los 60 hasta los 70+ años.
- **Selector de Edad**: Nueva interfaz de usuario con menú desplegable para seleccionar la edad de jubilación, actualizando instantáneamente la TAD y los resultados.
- **Contadores de Años Totales**: Implementación de indicadores visuales al lado del selector de edad que muestran la suma total de años de aporte (Historial Base + Futuro) para cada sistema de forma independiente.
- **Lógica Actuarial Mejorada**: El porcentaje de jubilación se calcula ahora multiplicando la TAD (según edad) por la suma real de años de servicios aportados detectados en el simulador.
