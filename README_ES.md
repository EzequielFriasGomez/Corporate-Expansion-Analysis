<p align="center">
  <img src="https://raw.githubusercontent.com/EzequielFriasGomez/Corporate-Expansion-Analysis/main/Presentaci%C3%B3n_Expansi%C3%B3n.gif" width="800"/>
</p>

# Auditoría de Rentabilidad y Expansión Corporativa (Mercado EE.UU.)

**Contexto del Proyecto** Este repositorio documenta el pipeline de datos y el análisis comercial de una empresa en fase de expansión. Utilizando un dataset simulado basado exclusivamente en el mercado de Estados Unidos, el objetivo fue auditar la salud financiera real del negocio, yendo más allá del volumen bruto de ventas para descubrir los márgenes netos de rentabilidad y definir la estrategia de apertura de nuevas sucursales.

**El Problema Comercial** A simple vista, la empresa presentaba un excelente volumen de facturación ($2.30 millones), pero la gerencia carecía de visibilidad sobre los costos operativos reales y el rendimiento segmentado. Necesitábamos descubrir qué regiones y qué categorías sostienen realmente a la empresa, y cuáles están generando pérdidas operativas ocultas.

**Arquitectura y Proceso (ETL & BI)** 1. **Python (Pandas):** Se construyó un pipeline de limpieza para purgar columnas irrelevantes, localizar el dataset al español (traducción de variables de negocio) y estandarizar formatos monetarios. Adicionalmente, se realizó ingeniería de características calculando el "Costo" operativo por transacción.
2. **Microsoft Power BI:** Ingesta del modelo limpio y cálculo dinámico de márgenes de rentabilidad utilizando expresiones DAX.

**Diagnóstico Comercial (Lo que dicen los datos)** El análisis expuso vulnerabilidades críticas en la estrategia comercial:
1. **El espejismo del Q4 vs. La rentabilidad del Q1:** El último trimestre del año concentra el mayor volumen de compras debido a las festividades y descuentos, pero destruye el margen comercial. El primer trimestre (Q1) demostró ser el más rentable, impulsado por *compras de necesidad* donde el consumidor no depende de las ofertas.
2. **El verdadero motor bicilíndrico:** La rentabilidad real no depende de un solo rubro. Tecnología lidera con el 50.79% de la ganancia neta, pero Insumos de Oficina opera como un segundo motor masivo con el 42.77%. Juntos sostienen el 93.56% del beneficio de la empresa.
3. **El lastre de los Muebles:** La categoría de Muebles genera volumen de ventas pero asfixia el margen global, representando apenas el 6.44% de la ganancia total. Este rubro se vende casi exclusivamente durante épocas de rebajas; la marca no es un referente en mobiliario, es una opción de saldo con altos costos logísticos.
4. **Brecha Regional:** La región Sur presenta un rendimiento alarmante, generando casi la mitad de las ventas y ganancias en comparación con la región Oeste, lo que exige una revisión del modelo de penetración en esa zona.

**Decisión Estratégica** 1. **Sector Muebles:** Se recomienda una auditoría urgente de la cadena logística para reducir costos de envío/almacenamiento, o bien una desinversión progresiva en el sector para inyectar ese capital directamente en las verticales eficientes.
2. **Optimización de Recursos:** Concentrar los esfuerzos de expansión en el binomio Tecnología-Insumos de Oficina. Pausar la apertura de sucursales genéricas en el Sur hasta entender el cuello de botella comercial, y consolidar la dominancia en las grandes urbes del Oeste y Este (New York, Los Ángeles, Seattle).

**Stack Tecnológico:** Python (Pandas) | Microsoft Power BI (DAX)
