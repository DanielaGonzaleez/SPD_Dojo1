# Documentacion Dojo D (Ejercicio 1)
![Tinkercad](https://github.com/DanielaGonzaleez/SPD_Dojo1/blob/main/ArduinoTinkercad.jpg)


## Integrantes
- Cristofori, Magalí
- De Maio, Juan Pablo
- Gonzalez, Daniela Leonor
- Martínez Balian, Francisco
- Rojas, Freddy
- Soto, Camila


## Proyecto: Contador binario.
![Tinkercad](https://github.com/DanielaGonzaleez/SPD_Dojo1/blob/main/SemaforoParaCiegos.png)


## Descripción
Este proyecto se hizo con la intención de crear un semáforo que tambien pueda serle útil a las personas no videntes. Para lograrlo utilizamos un piezo, que emite una secuencia de pitidos fuertes cuando el semáforo está en rojo. También se tomo la precaución de utilizar dos ejemplares de cada led para anteponerse a cualquier accidente con el primer ejemplar.  

## Función principal
Esta funcion se encarga de armar la secuencia de encendido y apagado de las led, asi como del piezo

LED_VERDE_UNO, LED_VERDE_DOS, LED_AMARILLO_UNO, LED_AMARILLO_DOS, LED_ROJO_UNO, LED_ROJO_DOS son #define que utilizamos para identificar mas facilmente a que led está asociado cada pin.

Las funciones prender, apagar y sonar_buzzer son funciones con parámetros formales, que obtienen valor a traves de los parámetros actuales, que son asignados cuando se llama a la funcion (Por ejemplo, en la linea 30). La funcion prender, como su nombre lo dice, va a prender dos led que nosotros le asignemos, durante el tiempo que le asignemos. La funcion apagar, hará lo contrario, las apagará. Por último, la función sonar_buzzer hará que el piezo suene medio segundo, y se detenga el mismo tiempo, esto se repetirá la cantidad de veces y a la frecuencia que nosotros le asignemos.

~~~ C++ (lenguaje en el que esta escrito)
{
  prender (LED_VERDE_UNO,LED_VERDE_DOS, 5000);
  apagar (LED_VERDE_UNO,LED_VERDE_DOS, 500);
  
  prender(LED_AMARILLO_UNO,LED_AMARILLO_DOS, 3000);
  apagar (LED_AMARILLO_UNO, LED_AMARILLO_DOS,500);
  
  prender (LED_ROJO_UNO,LED_ROJO_DOS,0);
  sonar_buzzer (10, 500);
  apagar (LED_ROJO_UNO, LED_ROJO_DOS,0);
  
  prender(LED_AMARILLO_UNO,LED_AMARILLO_DOS, 3000);
  apagar (LED_AMARILLO_UNO, LED_AMARILLO_DOS,500);
}
~~~

## :robot: Link al proyecto
- [proyecto](https://www.tinkercad.com/things/bkJ1uMIDWMM?sharecode=lWd_PFObZRYMuWyhXgv4QrPj9RyFbbjXB0uRiZ_1Gr4)

---
### Fuentes
- [Consejos para documentar](https://www.sohamkamani.com/how-to-write-good-documentation/#architecture-documentation).

- [Lenguaje Markdown](https://markdown.es/sintaxis-markdown/#linkauto).

- [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

- [Tutorial](https://www.youtube.com/watch?v=oxaH9CFpeEE).

- [Emojis](https://gist.github.com/rxaviers/7360908).

---
