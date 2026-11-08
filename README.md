# Examen del Parcial II: caso aplicado

IN1042 Aprendizaje Automático III, Grupo A7, Otoño 2026.

## Integrantes y quién hizo qué

| Integrante | Qué hizo |
|---|---|
| Juan Yael Vásquez Avelar | Cuaderno DEV, resultados y modelo de CardioRitmo (`ecg/`) |
| Emilio Frausto Ortiz | Cuaderno DEV, resultados y modelo de Compra Fácil Bajío (`resenas/`) |
| Rodrigo Rosales Díaz | Folletos y maquetas del PMV de los dos problemas (`ecg/folleto_ecg.pdf` y `resenas/folleto_resenas.pdf`) |

## Modelo elegido en cada problema

**Problema 1, CardioRitmo (tamizaje de latidos):** red LSTM con 4,385 parámetros. En la prueba logró sensibilidad de 99.5 %, especificidad de 99.7 % y AUC de 0.998, así que cumple las especificaciones del cliente. Archivo: `ecg/modelo/modelo_ecg.keras`.

**Problema 2, Compra Fácil Bajío (reseñas negativas):** bigramas con una red densa, con 480,033 parámetros. En la prueba logró exhaustividad de 92.4 %, precisión de 89.7 % y exactitud de 90.8 %, así que cumple las especificaciones del cliente. Archivos: `resenas/modelo/modelo_resenas.keras` y `resenas/modelo/vocabulario_bigramas.json`, el vocabulario que convierte el texto en la entrada del modelo.

## Estructura

```
├── README.md
├── ecg/
│   ├── DEV_ecg.ipynb
│   ├── resultados_ecg.csv
│   ├── modelo/
│   └── folleto_ecg.pdf
└── resenas/
    ├── DEV_resenas.ipynb
    ├── resultados_resenas.csv
    ├── modelo/
    └── folleto_resenas.pdf
```
