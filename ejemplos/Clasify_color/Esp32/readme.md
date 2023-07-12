1- INSTALACION DE LIBRERIAS:

La primera  libreria que debemos descargar es la  del sensor APDS9960. 
en este caso arduino tiene una libreria correspondiente al sensor creado por adafruit.

ya en el IDE de arduino procedemos a buscar  en el gestor de librerias dicho sensor asi: 


![apds9960](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/41412df2-d0cc-4c9d-9dbf-ac7879974747)

luego necesitamos la libreria de tensorflowlite para ESP32.
para obtenerla debemos ir al gestor de librerias y escribir "Tensorflow lite esp32"

![tensorflowesp32](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/77f8f2f4-b7fc-4ede-8b5d-cae3ae87d654)




2- CAPTURA DE DATOS PARA LE CREACION DEL DATASET:
Para la captura de los datos usaremos el sckech llamado "color_capture" que recopila los datos del sensor y envia esos valores a traves de comunicacion serial.

luego usaremos el programa "coolterm" para conectarnos a la placa y capturar los datos en un archivo .csv 

![cool](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/4d574ed8-ad1d-4f84-a640-3f8dcfb4bf5e)

en el programa nos remitiremos al apartado de configuracion en donde escojemos el COM correspondiente con la placa y 
los baudios a los que trasmite.

![cool2](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/cf1713ac-64a3-469f-999a-e538784458c8)

![cool3](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/d39dfc32-d03f-4cc2-b8d8-093a5ac3db40) 
