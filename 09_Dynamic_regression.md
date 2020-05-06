Modelos de regresión dinámica
================

Los modelos de pronóstico de suavización exponencial y ARIMAs son
estimdos **a través de observaciones pasadas**, pero **no permiten
incluir información exógena** a la serie (otras variables).

Por ejemplo, para pronosticar la demanda de energía eléctrica, podemos
implementar un ARIMA estacional. Sin embargo, cuánta energía se consume
en los hogares se ve afectada fuertemente por la temperatura ambiental
en ese momento. Con el SARIMA solo podríamos obtener la dinámica de la
propia serie, pero tal vez sería bueno incluir también como predictora a
la temperatura.

Recordando, un modelo de regresión tiene la forma general

\[y_{t}=\beta_{0}+\beta_{1} x_{1, t}+\cdots+\beta_{k} x_{k, t}+\varepsilon_{t}\]

donde \(y_t\) es la variable que queremos pronosticar, \(x_{k, t}\) son
las variables independientes que utilizábamos para

Y un modelo ARIMA
