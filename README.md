# esp-mos-max31865
Objetivo: leer temperatura con TP100 y módulo MAX31865 conectado a ESP8266 (1M) que tiene instalado Mongoose OS.

Se está siguiendo la guía  
https://mongoose-os.com/docs/mongoose-os/quickstart/setup.md

apps - proyectos de ejemplo  
https://github.com/mongoose-os-apps

libs - bibliotecas para sensores, comunicación, etc.  
https://github.com/mongoose-os-libs

Problema al flashear ESP8266 con 1M de memoria (firmware no cabe)  
https://github.com/cesanta/mongoose-os/issues/307  
https://forum.mongoose-os.com/discussion/3625/unable-to-build-for-esp-wroom-02  
https://community.mongoose-os.com/t/unable-to-flash-esp8266-1m/949  
Solución, compilar con esta instrucción  
```mos build --platform esp8266 --build-var FLASH_SIZE=1048576 --clean```

## Info sobre MAX31865
El módulo  
https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier?view=all

Bliblioteca para Arduino. Alto nivel de exactitud, pero ocupa mucho espacio  
https://github.com/drhaney/pt100rtd

En el foro no hay respuestas  
https://forum.mongoose-os.com/discussion/2015/spi-communication-with-api-spi-js  
https://community.mongoose-os.com/t/i-create-one-library-from-arduino-but-its-getting-error-when-include/980  

Probar esta lib  
https://github.com/rpo19/arduino-adafruit-max31865  
