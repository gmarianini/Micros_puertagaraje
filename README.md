# Micros_puertagaraje

Durante este proyecto hemos realizado un programa encargado de gestionar el acceso a un parking mediante un sensor infrarrojo de entrada y otro de salida. Se han añadido funcionalidades adicionales como el encendido automático de las luces cuando se esta haciendo de noche con la utilización de un sensor LDR. Para ello el programa se debe realizar en lenguaje C e implementado en un microcontrolador STM32F411.

Sensores ultrasónicos HC-SR04:

    -Mide distancias utilizando dos sensores ultrasónicos (entrada y salida).
    
    -Cambia automáticamente el flanco (ascendente/descendente) para capturar el inicio y fin del pulso del sensor, determinando el tiempo de vuelo del ultrasonido.

Control de motor:

    -Controla el ángulo de un motor según las distancias medidas por los sensores.
    
    -Actúa como una compuerta, abriendo o cerrando en función de las mediciones.

Indicadores LED:
    -Enciende o apaga LEDs en función de los valores medidos por el ADC y los sensores ultrasónicos.

Mediciones optimizadas:

    -Utiliza DMA para leer datos del ADC sin interrumpir el flujo principal del programa.
    
    -Gestiona los sensores y calcula las distancias sin bloqueos, aprovechando interrupciones.
