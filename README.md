# Challenge_TelecomX_Kari
Desafio del programa ONE para poner en practica conceptos pandas, matpolit y numpy
# Informe Final – Telecom X: Análisis de Evasión (Churn)

**Objetivo.** Comprender los factores asociados a la evasión de clientes del servicio de internet Telecom X para apoyar estrategias de retención y nutrir futuros modelos predictivos.

## Limpieza y Tratamiento de Datos se realizo lo siguiente
# - Se normalizaron las columnas que eran diccionarios para mejor manejo y ananlisis de los datos
# - Estandarización de la variable objetivo: conversión a binaria (0/1) en **{col_churn_es}**.
# - Revisión de consistencia lógica entre servicios (p.ej., Internet y add-ons).
# - Normalización de etiquetas categóricas cuando corresponde (contratos, métodos de pago, etc.).
# - Manejo de *missing values* en cargos totales para tenure=0 (clientes nuevos).

# Se realizo un analisis exploratorio de los datos a fines de identificar patrones, de lo cual surgieron las siguientes observaciones:
# - No se aprecia tendencia a laevasion de clientes por genero
# - Se aprecia que la evacion o cancelacion de los clientes esta fuertemente determinado por quienes tienen contrato mes a mes y por quienes pagan con chequera electronica
# - Se aprecia que la evacion o cancelacion se da mas en el tipo de internet por fibra optica y quienes tienen servicio telefonico

<img width="581" height="534" alt="image" src="https://github.com/user-attachments/assets/2b39d974-9ee0-4bab-b45f-1eff940f4018" />
<img width="606" height="587" alt="image" src="https://github.com/user-attachments/assets/1d05cef4-343e-44b5-8e6b-e35ac4c91fe4" />


# insights 
# - Los cargos totales entre 0 y 2000 tienen mas tasa de cancelacion
# - Los cargos mensuales mas altos entre 58 y 95 suelen tener mayor tasa de cancelacion
# - Las personas con antiguedad entre 2 meses y 28 meses son quienes mas ancelan el servicio

## Recomendaciones

# -**Retención temprana:** diseñar onboarding, descuentos iniciales o beneficios en los primeros meses si la fuga es temprana.
# -**Segmentación por precio:** revisar planes con cargos mensuales más altos; ofrecer **bundles** o valor agregado para reducir sensibilidad al precio.
# -**Alertas proactivas:** monitoreo de tickets/soporte y degradación de servicio (especialmente en clientes con Internet de alto costo).
# -**Fidelización por contrato:** incentivar contratos de mayor plazo con beneficios transparentes (evitar fricción al migrar).
# -**Optimizar métodos de pago:** ya que el método cheque electronico concentra más churn, revisar UX de cobro, recordatorios y fallas de pago.
