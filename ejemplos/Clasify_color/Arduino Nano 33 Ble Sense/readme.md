1- INSTALACION DE LIBRERIAS:
Para empezar necesitamos agregar nuestra placa al IDE de arduino 
para esto debemos entrar al gestor de tarjetas y buscar lo siguiente "Arduino Mbed OS nano Boards" e instalamos.

![mbed boards](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/39af93ca-2595-4340-a88a-f2c79feca8a3)



La segunda libreria que usaremos es la libreria del sensor APDS9960.
en este caso arduino tiene una libreria correspondiente al sensor ya incorporado de la placa arduino nano 33 ble sense.

ya en el IDE de arduino procedemos a buscar  en el gestor de librerias dicho sensor asi:

![apds](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/bdf174d4-73e4-42af-b42c-e22ce3874424)

luego necesitamos la libreria de tensorflowlite para arduino.
para obtenerla debemos descargarla desde internet ya que el gestor de librerias de arduino no tiene disponible esta libreria.
la pagina para descargar la libreria es https://github.com/tensorflow/tflite-micro-arduino-examples
dentro de la pagina procederemos a descargar el archivo .ZIP de la libreria.

![github](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/a5f24dba-4db9-49e3-ae7c-1396705c0fed)

finalmente debemos agregarla a el IDE de arduino siguiendo estos pasos:
  - en la pestaña de "programa" nos dirigimos a incluir biblioteca .zip y seleccionamos el archivo que descargamos.

![agregar](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/9c2a1924-da81-4d92-8ff4-9118eac5fd64)

2- CAPTURA DE DATOS PARA LE CREACION DEL DATASET:
Para la captura de los datos usaremos el sckech llamado "color_capture" que recopila los datos del sensor y envia esos valores a traves de comunicacion serial.

luego usaremos el programa "coolterm" para conectarnos a la placa y capturar los datos en un archivo .csv 

![cool](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/4d574ed8-ad1d-4f84-a640-3f8dcfb4bf5e)

en el programa nos remitiremos al apartado de configuracion en donde escojemos el COM correspondiente con la placa y 
los baudios a los que trasmite.


![cool2](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/cf1713ac-64a3-469f-999a-e538784458c8)

![cool3](https://github.com/antuki29/Tutorial_tinyML_Udenar/assets/84738230/d39dfc32-d03f-4cc2-b8d8-093a5ac3db40)


3- DISEÑO DE LA RED NEURONAL:
con el dataset listo se procede a realizar el diseño de nuestra red neuronal.
la herramienta que usamos el Colab ya que nos permite entrener modelos de machine learning en un escritorio remoto con mejores capacidades de computo.
Colab proporciona un cuaderno Jupyter que nos permite ejecutar codigo en un navegador web.

este cuaderno de Jupyter se divide en:
* configuracion de librerias necesarias.
* cargar y leer los archivos .CSV del dataset.
* analizar y preparar los datos.
* construir y entrenar el modelo.
* convertir el modelo entrenedo a tensorflow lite.




