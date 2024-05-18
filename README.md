# Detección de Fraudes en Transacciones Financieras

Este proyecto tiene como objetivo principal investigar la viabilidad del entrenamiento incremental en modelos de aprendizaje automático y profundo utilizando un conjunto de datos de transacciones con tarjeta de crédito. Se busca detectar transacciones fraudulentas en un entorno cambiante y dinámico.

## Descripción del Dataset

El dataset utilizado en este proyecto consiste en transacciones simuladas con tarjeta de crédito, que incluyen transacciones legítimas y fraudulentas realizadas entre el 1 de enero de 2019 y el 31 de diciembre de 2020. El dataset cubre transacciones de tarjetas de crédito de 1000 clientes en un conjunto de 800 comercios. Contiene un total de 68 características, incluidas características originales y características generadas.

- [Conjunto de datos de transacciones financieras](https://drive.google.com/file/d/1_baHRvvi2OKAKdRnHArCGI9ZpYCxAiMg/view?usp=sharing)

## Metodologías y Algoritmos Utilizados

Para abordar este problema, se han explorado las siguientes metodologías y algoritmos:

1. **Entrenamiento Incremental:** Se ha investigado la viabilidad del entrenamiento incremental en modelos de aprendizaje automático y profundo para adaptarse a los cambios en la distribución de datos.

2. **Modelos de Aprendizaje Automático:** Se han utilizado modelos de LightGBM, XGBoost, Random Forest, y Máquinas de Vectores de Soporte (SVM) para clasificar las transacciones como legítimas o fraudulentas.

3. **Redes Neuronales Artificiales (ANN):** Se ha implementado una red neuronal artificial para explorar su capacidad para detectar transacciones fraudulentas en un entorno cambiante.

## Características Finales

Después de eliminar las columnas innecesarias, estas son las características finales que se utilizaron en el análisis:

1. **amt:** Monto de la transacción.
2. **zip:** Código postal del cliente.
3. **lat:** Latitud del lugar de la transacción.
4. **long:** Longitud del lugar de la transacción.
5. **city_pop:** Población de la ciudad donde se realizó la transacción.
6. **is_fraud:** Etiqueta que indica si la transacción fue fraudulenta o no.
7. **amt_month:** Monto promedio de la transacción por mes.
8. **amt_year:** Monto promedio de la transacción por año.
9. **amt_month_shopping_net_spend:** Monto promedio gastado en compras en línea por mes.
10. **count_month_shopping_net:** Número promedio de transacciones en compras en línea por mes.
11. **first_time_at_merchant:** Indicador booleano que señala si es la primera vez que el cliente realiza una transacción en ese comercio.
12. **amt_month_misc_net_spend:** Monto promedio gastado en compras misceláneas por mes.
13. **count_month_misc_net_trx:** Número promedio de transacciones misceláneas por mes.
14. **amt_month_grocery_pos_spend:** Monto promedio gastado en tiendas de comestibles (compras en puntos de venta) por mes.
15. **count_month_grocery_pos_trx:** Número promedio de transacciones en tiendas de comestibles (compras en puntos de venta) por mes.
16. **amt_month_entertainment_spend:** Monto promedio gastado en entretenimiento por mes.
17. **count_month_entertainment_trx:** Número promedio de transacciones de entretenimiento por mes.
18. **amt_month_gas_transport_spend:** Monto promedio gastado en gasolina y transporte por mes.
19. **count_month_gas_transport_trx:** Número promedio de transacciones de gasolina y transporte por mes.
20. **amt_month_misc_pos_spend:** Monto promedio gastado en compras misceláneas (compras en puntos de venta) por mes.
21. **count_month_misc_pos_trx:** Número promedio de transacciones misceláneas (compras en puntos de venta) por mes.
22. **amt_month_grocery_net_spend:** Monto promedio gastado en tiendas de comestibles (compras en línea) por mes.
23. **count_month_grocery_net_trx:** Número promedio de transacciones en tiendas de comestibles (compras en línea) por mes.
24. **count_month_shopping_net_trx:** Número promedio de transacciones de compras en línea por mes.
25. **amt_month_shopping_pos_spend:** Monto promedio gastado en compras en línea (compras en puntos de venta) por mes.
26. **count_month_shopping_pos_trx:** Número promedio de transacciones de compras en línea (compras en puntos de venta) por mes.
27. **amt_month_food_dining_spend:** Monto promedio gastado en comida y restaurantes por mes.
28. **count_month_food_dining_trx:** Número promedio de transacciones de comida y restaurantes por mes.
29. **amt_month_personal_care_spend:** Monto promedio gastado en cuidado personal por mes.
30. **count_month_personal_care_trx:** Número promedio de transacciones de cuidado personal por mes.
31. **amt_month_health_fitness_spend:** Monto promedio gastado en salud y fitness por mes.
32. **count_month_health_fitness_trx:** Número promedio de transacciones de salud y fitness por mes.
33. **amt_month_travel_spend:** Monto promedio gastado en viajes por mes.
34. **count_month_travel_trx:** Número promedio de transacciones de viajes por mes.
35. **amt_month_kids_pets_spend:** Monto promedio gastado en artículos para niños y mascotas por mes.
36. **count_month_kids_pets_trx:** Número promedio de transacciones de artículos para niños y mascotas por mes.
37. **amt_month_home_spend:** Monto promedio gastado en artículos para el hogar por mes.
38. **count_month_home_trx:** Número promedio de transacciones de artículos para el hogar por mes.
39. **is_weekend:** Indicador booleano que señala si la transacción se realizó durante el fin de semana.
40. **is_night:** Indicador booleano que señala si la transacción se realizó durante la noche.
41. **customer_num_transactions_1_day:** Número total de transacciones del cliente en un día.
42. **customer_num_transactions_7_day:** Número total de transacciones del cliente en una semana.
43. **customer_num_transactions_30_day:** Número total de transacciones del cliente en un mes.
44. **customer_avg_amount_1_day:** Monto promedio de transacciones del cliente en un día.
45. **customer_avg_amount_7_day:** Monto promedio de transacciones del cliente en una semana.
46. **customer_avg_amount_30_day:** Monto promedio de transacciones del cliente en un mes.
47. **trans_hour:** Hora del día en que se realizó la transacción (en horas).
48. **trans_day:** Día de la semana en que se realizó la transacción.
49. **terminal_num_transactions_1_day:** Número total de transacciones en un terminal en un día.
50. **terminal_num_transactions_7_day:** Número total de transacciones en un terminal en una semana.
51. **terminal_num_transactions_30_day:** Número total de transacciones en un terminal en un mes.

Estas características fueron seleccionadas para su inclusión en el análisis final debido a su potencial para contribuir a la detección de transacciones fraudulentas.

## Evaluación y Monitoreo

Se han utilizado diversas métricas de evaluación, como precisión, recall, F1-score, y curvas ROC-AUC, para evaluar el rendimiento de los modelos en la detección de transacciones fraudulentas. Además, se ha implementado un sistema de monitoreo continuo para detectar y abordar el data drift en tiempo real.
