# Bank-Credit---Logistic-Regression
## Proyecto para determinar si un cliente será apto para un depósito a plazo fijo o no según las variables disponibles con un modelo de regresión logística

## Información del Dataset
El dataset utilizado en este proyecto contiene las siguientes variables:

- **job:** tipo de trabajo (categórico: "admin.", "blue-collar", "entrepreneur", "housemaid", "management", "retired", "self-employed", "services", "student", "technician", "unemployed", "unknown")
- **marital:** estado civil (categórico: "divorced", "married", "single", "unknown"; nota: "divorced" incluye divorciado y viudo)
- **education:** nivel educativo (categórico: "basic.4y", "basic.6y", "basic.9y", "high.school", "illiterate", "professional.course", "university.degree", "unknown")
- **default:** tiene créditos en mora? (categórico: "no", "yes", "unknown")
- **housing:** tiene préstamo hipotecario? (categórico: "no", "yes", "unknown")
- **loan:** tiene préstamo personal? (categórico: "no", "yes", "unknown")

Relacionados con el último contacto de la campaña actual:

- **contact:** tipo de comunicación de contacto (categórico: "cellular", "telephone")
- **month:** mes del último contacto del año (categórico: "jan", "feb", "mar", ..., "nov", "dec")
- **day_of_week:** día del último contacto de la semana (categórico: "mon", "tue", "wed", "thu", "fri")
- **duration:** duración del último contacto en segundos (numérico). Nota importante: este atributo afecta altamente la variable objetivo (por ejemplo, si duration=0 entonces y="no"). Sin embargo, la duración no se conoce antes de realizar una llamada. Por lo tanto, este input solo debe incluirse para propósitos de referencia y debe descartarse si la intención es tener un modelo predictivo realista.

Otras variables:

- **campaign:** número de contactos realizados durante esta campaña y para este cliente (numérico, incluye el último contacto)
- **pdays:** número de días que han pasado desde que el cliente fue contactado por última vez en una campaña anterior (numérico; 999 significa que el cliente no fue contactado previamente)
- **previous:** número de contactos realizados antes de esta campaña y para este cliente (numérico)
- **poutcome:** resultado de la campaña de marketing anterior (categórico: "failure", "nonexistent", "success")

Atributos del contexto social y económico:

- **emp.var.rate:** tasa de variación del empleo - indicador trimestral (numérico)
- **cons.price.idx:** índice de precios al consumidor - indicador mensual (numérico)
- **cons.conf.idx:** índice de confianza del consumidor - indicador mensual (numérico)
- **euribor3m:** tasa euribor a 3 meses - indicador diario (numérico)
- **nr.employed:** número de empleados - indicador trimestral (numérico)

## Variable de Salida (Objetivo Deseado)
- **y:** el cliente ha suscrito un depósito a plazo fijo? (binario: "yes", "no")
