##      Documentos para FreeRTOS

###     eBook de Elektor

  En este directorio se encuentra, para mi, el mejor tutorial escrito especificamente para ESP32 bajo Arduino o PlatformIO
  En el directorio Elektor, se encontrará el mismísimo libro y aparte, se encuentran los códigos de todos los ejercicios propuestos en el libro.

###     Documentarción de _freertos.org_

  La documentación definitiva es la de la propia _freertos.org_ que es la más detallada; sin embargo, posee un inconveniente: _FreeRTOS_  se usa bajo múltiples plataformas, con lo cual la documentación que se presenta aquí es la genérica que, si bien es la definitiva en caso de duda, no está adaptada a los detalles de cada una de las implementaciones (por ejemplo, el ESP32 posee dos núcleos, por lo cual muchas funciones de _FreeRTOS_ están levemente modificadas para adaptarse a este hecho).

  [FreeRTOS Documentation](https://www.freertos.org/Documentation/RTOS_book.html)

###     Ejemplos de biblioteca de ESP32 incluida bajo Arduino

  La implementación de ESP32 bajo Arduino se realiza mediante bibliotecas incluidas en el mismo Arduino; se puede ver la impementación de dichas bibliotecas con ejemplos yendo a _github_ en el siguiente link

  [arduino-esp32](https://github.com/espressif/arduino-esp32/tree/master)

  Dentro de ese link, se encontrarán ejemplos de aplicación de todas las bibliotecas incluidas

  [arduino-esp32 libraries examples](https://github.com/espressif/arduino-esp32/tree/master/libraries/ESP32/examples)

  Dentro del anterior, puede encontrar las especificas de FreeRTOS

  [arduino-esp32 libraries examples FreeRTOS](https://github.com/espressif/arduino-esp32/tree/master/libraries/ESP32/examples/FreeRTOS)

###     Conclusión

  Se sugiere, entonces:

  1. Basarse en la documentación de Elektor
  2. En caso de duda de alguna de las funciones, ver el detalle en la descripción de _freertos.org_
  3. Puede ser que alguno de los ejemplos de la biblioteca de ESP32 sea útil, especialmente para comprender los tres casos de comunicación entre tareas que posee _FreeRTOS_ como son: _Mutex_, _Queue_, _Semaphore_






