# Configuración de la librería TFT_eSPI para funcionamiento de la ESP32 con la ST7789
 Instalar la librería TFT_eSPI ya sea desde el administrador de Arduino o del siguiente link como ZIP
 [Link]( https://github.com/Bodmer/TFT_eSPI.git  )

 ![img1](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/1.%20Libreria%20TFT_eSPI.png)
 Del repositorio de librerías de Arduino del ordenado abrimos la librería instalada y procedeos a abrir el archivo User_Setup.h 
 ![img2](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/2.%20Carpeta%20de%20la%20libreria.png)

Una vez abierto procedemos primero a activar las siguientes opciones en cada sección 
// Section 1. Call up the right driver file and any options for it
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img3](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/3.%20Configuracion%20del%20Setup.png)
// Section 2. Define the pins that are used to interface with the display here
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img4](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/4.%20Configuracion%20del%20Setup%202.png)
// Section 3. Define the fonts that are to be used here
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img5](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/5.%20Configuracion%20del%20Setup%203.png)
// Section 4. Other options
En esta sección debe estar activado solo los siguientes drivers los demás deben estar comentados
![img6](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/6.%20Configuracion%20del%20Setup%204.png)
# Animación de un gif
Una vez configurado la librería comenzamos con el descargar un gif del internet o crearlo con imágenes como se ha hecho, una vez creado el o descargado el gif nos dirigimos a este enlace para dividir lo en imágenes JPG
[Link]( https://ezgif.com/ )
En la opción del Split 
![img7](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/7.%20Separacion%20de%20imagenes%20GIF.png)
Una vez ya cargada el Gif y dividida descargamos la carpeta como ZIP como muestra la imagen
![img8](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/8.%20Descargar%20el%20ZIP.png)
Una vez descargada en el lugar que se necesite descomprimimos la carpeta y abrimos el siguiente programa
![img9](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/9.%20Programa.png)
Este programa se encuentra en el mismo repositorio de GitHub 
Al abrir el programa se desplegará la siguiente ventana 
![img10](https://github.com/ArtilRobotics/TFT_eSPI/blob/1b68e8cdbab2fa25da6d24ffefd2fb812fb9d8c7/Imagenes/10.%20Convertir%20imagenes%20a%20archivo%20.h.png)
Primero ponemos el nombre del archivo .h que se generara para posteriormente seleccionar la carpeta y se generara el archivo .h en la carpeta para posteriormente ejecutar el archivo. ino que se encuentra en el repositorio.
Tener en cuenta que la conexión en la ESP32 con la ST7789 es de la siguiente manera para que funcione correctamente:
| ESP32 WROOM | ST7789 |
| ------------- | ------------- |
| GND  | GND |
|3V3 AND BLK| VCC |
|G18| SCL|
|G23| SDA|
|G4| RES|
|G2| DC|
|VCC| BLK|