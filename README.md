# PWM_FPGA
Gael Cumplido Mendoza - A01029238

Práctica: Módulo PWM para Control de Servomotor en FPGA DE10-Lite

📌 Descripción

El módulo PWM generará una señal con una frecuencia de 50 Hz (período de 20 ms), adecuada para el control de servomotores, El duty cycle (ancho de pulso) determinará la posición del servomotor, por lo que si es un duty cycle bajo el servomotor tenrda un angulo de inclinacion bajo

1 ms → Posición mínima

1.5 ms → Posición central

2 ms → Posición máxima

Se usarán los botones de la FPGA para aumentar o disminuir el duty cycle en incrementos pequeños.

⚙️ Requisitos

Tarjeta FPGA DE10-Lit

Software Intel Quartus Prime Lite

Servomotor compatible con señal PWM (ejemplo: SG90, MG995)

Fuente de alimentación externa para el servomotor (5V)

Conexiones de cables jumper


📂 Estructura del Proyecto

/PWM

│── PWM_servo.v # Módulo principal que implementa las funciones.

│── PWM_tb.v # Testbench para simulación

│── PWM.qpf # Archivo del proyecto en Quartus

│── PWM.qsf # Archivo de configuración del FPGA

│── debouncer2.v # Módulo para eliminar ruido de los botones

│── d_ff.v # Módulo que implementa el flip-flop tipo D

│── clkdiv.v # Módulo que implementa el clock dvider para ajustar el tiempo de ejecución.

│── README.md # Este archivo
