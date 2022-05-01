# Configuración de la librería TFT_eSPI para funcionamiento de la ESP32 con la ST7789
 Instalar la librería TFT_eSPI ya sea desde el administrador de Arduino o del siguiente link como ZIP
 [Link]( https://github.com/Bodmer/TFT_eSPI.git  )

 ![img1]()
 Del repositorio de librerías de Arduino del ordenado abrimos la librería instalada y procedeos a abrir el archivo User_Setup.h 
 ![img2]()

Una vez abierto procedemos primero a activar las siguientes opciones en cada sección 
// Section 1. Call up the right driver file and any options for it
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img3]()
// Section 2. Define the pins that are used to interface with the display here
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img4]()
// Section 3. Define the fonts that are to be used here
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img5]()
// Section 4. Other options
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img6]()
# Animación de un gif
Una vez configurado la librería comenzamos con el descargar un gif del internet o crearlo con imágenes como se ha hecho, una vez creado el o descargado el gif nos dirigimos a este enlace para dividir lo en imágenes JPG
[Link]( https://ezgif.com/ )
En la opción del Split 
![img7]()
Una vez ya cargada el Gif y dividida descargamos la carpeta como ZIP como muestra la imagen
![img8]()
Una vez descargada en el lugar que se necesite descomprimimos la carpeta y abrimos el siguiente programa
![img9]()
Este programa se encuentra en el mismo repositorio de GitHub 
Al abrir el programa se desplegará la siguiente ventana 
![img10]()
Primero ponemos el nombre del archivo .h que se generara para posteriormente seleccionar la carpeta y se generara el archivo .h en la carpeta para posteriormente ejecutar el archivo. ino que se encuentra en el repositorio.
Tener en cuenta que la conexión en la ESP32 con la ST7789 es de la siguiente manera para que funcione correctamente:
ESP32 WROOM	  ST7789
GND	          GND
3V3 AND BLK	  VCC
G18	          SCL
G23	          SDA
G4	          RES
G2	          DC
VCC	          BLK

