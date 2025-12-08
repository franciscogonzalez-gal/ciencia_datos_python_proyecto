# Ciencia de Datos en Python - Proyecto Final

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Descripción

Este proyecto es el trabajo final del curso de Ciencia de Datos en Python. Se realiza un análisis de datos sobre reservas de hoteles, incluyendo exploración de datos, visualización y modelos de regresión lineal.

## Autores

- Francisco González
- Vencent Martinez

## Dataset

El proyecto utiliza el dataset `hotel_bookings.csv`, que contiene información sobre reservas de hoteles. A continuación se describen las variables principales:

### Variables del Dataset

| Variable | Descripción |
|----------|-------------|
| `hotel` | Tipo de hotel (City Hotel, Resort Hotel) |
| `is_canceled` | Indica si la reserva fue cancelada (0 = no, 1 = sí) |
| `lead_time` | Días entre la reservación y la fecha de llegada |
| `arrival_date_year` | Año de llegada del huésped |
| `arrival_date_month` | Mes de llegada |
| `arrival_date_week_number` | Número de semana del año de llegada |
| `arrival_date_day_of_month` | Día del mes de llegada |
| `stays_in_weekend_nights` | Noches de fin de semana de la estancia |
| `stays_in_week_nights` | Noches entre semana de la estancia |
| `adults` | Cantidad de adultos en la reserva |
| `children` | Cantidad de niños en la reserva |
| `babies` | Cantidad de bebés en la reserva |
| `meal` | Tipo de paquete de comidas (BB, HB, FB, SC) |
| `country` | País de origen del huésped |
| `market_segment` | Segmento de mercado |
| `distribution_channel` | Canal de distribución de la reserva |
| `is_repeated_guest` | Indica si es un huésped recurrente |
| `previous_cancellations` | Número de cancelaciones previas |
| `previous_bookings_not_canceled` | Reservas previas no canceladas |
| `reserved_room_type` | Tipo de habitación reservada |
| `assigned_room_type` | Tipo de habitación asignada |
| `booking_changes` | Cambios realizados a la reserva |
| `deposit_type` | Tipo de depósito |
| `agent` | ID del agente de viajes |
| `company` | ID de la compañía |
| `days_in_waiting_list` | Días en lista de espera |
| `customer_type` | Tipo de cliente |
| `adr` | Tarifa diaria promedio (Average Daily Rate) |
| `required_car_parking_spaces` | Espacios de estacionamiento requeridos |
| `total_of_special_requests` | Número de solicitudes especiales |
| `reservation_status` | Estado de la reserva |
| `reservation_status_date` | Fecha del estado de reserva |

## Análisis Realizado

El proyecto incluye:

1. **Exploración de Datos**: Análisis descriptivo del dataset de reservas de hoteles.
2. **Modelos de Regresión Lineal**: 
   - Implementación manual de regresión lineal
   - Implementación usando `sklearn`
3. **Comparación de Modelos**: Evaluación mediante Error Cuadrático Medio (MSE) en conjunto de validación.

## Requisitos

Para ejecutar este proyecto necesitas:

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

Puedes instalar las dependencias con:

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

## Uso

1. Clona el repositorio:
   ```bash
   git clone https://github.com/franciscogonzalez-gal/ciencia_datos_python_proyecto.git
   ```

2. Navega al directorio del proyecto:
   ```bash
   cd ciencia_datos_python_proyecto
   ```

3. Abre el notebook de Jupyter:
   ```bash
   jupyter notebook proyecto.ipynb
   ```

4. Ejecuta las celdas del notebook para reproducir el análisis.

## Estructura del Proyecto

```
ciencia_datos_python_proyecto/
├── README.md              # Este archivo
├── LICENSE.txt            # Licencia CC0 1.0 Universal
├── hotel_bookings.csv     # Dataset de reservas de hoteles
└── proyecto.ipynb         # Notebook principal con el análisis
```

## Resultados

Los modelos de regresión lineal fueron evaluados y comparados:

- Para la variable `children`: El mejor modelo fue sklearn con MSE = 3231.04
- Para la variable `adults`: El mejor modelo fue sklearn con MSE = 3473.46

## Licencia

Este proyecto está bajo la licencia [CC0 1.0 Universal](LICENSE.txt) (Dominio Público).
