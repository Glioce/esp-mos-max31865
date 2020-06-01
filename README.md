# esp-mos-max31865
Objetivo: leer temperatura con TP100 y módulo MAX31865 conectado a ESP8266 (1M) que tiene instalado Mongoose OS.

Se están siguiendo guías  
https://mongoose-os.com/docs/mongoose-os/quickstart/setup.md

apps - proyectos de ejemplo  
github.com/mongoose-os-apps

libs - bibliotecas para sensores, comunicación, etc.  
https://github.com/mongoose-os-libs

Problema al flashear ESP8266 con 1M de memoria (firmware no cabe)  
https://github.com/cesanta/mongoose-os/issues/307  
https://forum.mongoose-os.com/discussion/3625/unable-to-build-for-esp-wroom-02  
Solución, compilar con esta instrucción  
```mos build --platform esp8266 --build-var FLASH_SIZE=1048576 --clean```

## Info sobre MAX31865
...
