# Laboratorio 4 Red y Máquinas Virtuales
## Elaborado por: Laura Rodriguez y Diana Bernal
## 1. Conexión con switch basico cisco 2960
### 1.1 Configuración de conexion serial

+ En primer lugar, se procedió a realizar la conexión por screen como se puede evidenciar en seguida:

![Imagen de WhatsApp 2025-09-29 a las 20 55 37_49722885](https://github.com/user-attachments/assets/d92a2456-2851-4a05-942a-3316a7f0e826)

<strong> Figura 1. </strong> Conexión vía screen por la terminal de Ubuntu.

### 1.2 Configuración del Cisco 2960

+ Enseguida, se procedió a realizar su configuración básica y la configuración de la Vlan 10 como se puede observar a continuación:
  
![Imagen de WhatsApp 2025-09-24 a las 21 30 53_d94921c0](https://github.com/user-attachments/assets/67bcdf97-4707-4f7a-a341-1141b23546f0)

<strong> Figura 2. </strong> Conexión básica Cisco 2960 (Visualización de comandos en Cisco).

![Imagen de WhatsApp 2025-09-29 a las 22 14 43_157aa5f3](https://github.com/user-attachments/assets/4b4b3348-6a87-44d6-bc8d-9c0295e5bf9f)

<strong> Figura 3. </strong> Configuración Vlan 10.

![Imagen de WhatsApp 2025-09-29 a las 21 03 50_1c811e57](https://github.com/user-attachments/assets/b9d478a6-7781-48a0-bca2-c250e994c713)

<strong> Figura 4. </strong> Configuración de la Vlan denominada (PcMonitor).

### 1.3 Configuración de los Dispositivos a conectar por medio del switch

#### 1.3.1 Configuración de la Rasberry

+ Para esta sección, lo que se realizó fue el proceso de configuración de red para la Rasberry con el objetivo de que pueda enviar y recibir información hacía los otros dispositivos por medio del switch:

![Imagen de WhatsApp 2025-09-29 a las 21 46 35_a6c2f22c](https://github.com/user-attachments/assets/aa501afd-fc58-429a-b26c-40d29829cbd8)

<strong> Figura 5. </strong> Configuración de la Rasperry.

#### 1.3.2 Configuración de IP del Pc Monitor

+ En primer lugar, se verificó que el PC tuviera una IP de Ethernet y se procedió a asignar una nueva. Esto con el objetivo de que todos los dispositivos esten en el en el mismo rango y la máscara de subred para poderse interconectar: 
  
![Imagen de WhatsApp 2025-09-29 a las 21 49 57_ed990489](https://github.com/user-attachments/assets/11c8de8d-8f85-41df-9337-a0a024cfd370)

<strong> Figura 6. </strong> Configuración del Pc Monitor.

+ En segundo lugar, se verificó con el comando de "Ping" que hubiera conexión entre la Raspberry y el Pc Monitor como se puede visualizar en las siguientes imagenes:

![Imagen de WhatsApp 2025-09-29 a las 21 47 42_15998f99](https://github.com/user-attachments/assets/0845f2d1-9fc2-47e1-b057-5a844821b997)

<strong> Figura 7. </strong> Verificación del comando ping para Pc Monitor (1).

![Imagen de WhatsApp 2025-09-29 a las 21 51 34_5f5fac10](https://github.com/user-attachments/assets/da95e5c8-aebc-4071-b520-0c46ca91bd8e)

<strong> Figura 8. </strong>  Verificación del comando ping para Pc Monitor (2).

#### 1.3.3 Verificación de conexión con el PC del ETM 

+ En tercer lugar, es posible visualizar como se hace conexión con el computador del ETM de la siguiente forma:
  
![Imagen de WhatsApp 2025-10-17 a las 07 55 06_e445cb73](https://github.com/user-attachments/assets/9832bf6e-3175-4053-b46b-5fd3abc04355)

<strong> Figura 9. </strong>  Verificación del comando ping para Pc ETM (2).

#### 1.3.4 Análisis de Redes (NMAP)

+ En cuarto lugar, se puede observar como se realizó un escaneo de red con el comando "NMAP" :

![Imagen de WhatsApp 2025-10-17 a las 07 52 59_6b7d6e1e](https://github.com/user-attachments/assets/92c223e5-a57a-4a17-84fd-39dacb79c7b7)

<strong> Figura 10. </strong> Uso del comando NMAP.

#### 1.3.5 Envío de Archivos de un Dispositivo fuente a un Dispositivo destino

Para esta sección no se pudo realizar el proceso completo:

![Imagen de WhatsApp 2025-10-17 a las 07 55 15_38adcf40](https://github.com/user-attachments/assets/4675740f-dffa-4fdd-a19d-5e79a92da3e1)

<strong> Figura 11. </strong> El puerto 22 se encuentra cerrado.

### 1.4 Instalación de las Maquinas Virtuales:

#### 1.4.1 Instalación de Ubuntu en Maquina Virtual:

#### 1.4.2  Instalación de Centos en Maquina Virtual:


#### 1.4.3  Instalación de Alpine en Maquina Virtual:

+ En primer lugar, se realizó la instalación del Terminal de Ubuntu, atraves de QEMU:

+ Luego, se creó el directorio para la máquina virtual:
  
<img width="1600" height="471" alt="image" src="https://github.com/user-attachments/assets/07f8891f-1413-4074-824a-fc2064511a46" />

+ Enseguida, se creo el disco virtual:
  
<img width="1600" height="80" alt="image" src="https://github.com/user-attachments/assets/dd2a7095-5b8c-49f2-90ac-565281aba26e" />

+ Iniciamos la instalación de Alpine:
  
<img width="1533" height="937" alt="image" src="https://github.com/user-attachments/assets/c23c8ef1-aaf7-4fc5-885e-575bde5723a2" />

<img width="1310" height="917" alt="image" src="https://github.com/user-attachments/assets/58c89697-c2ec-4211-845b-2662186458ed" />

+ Una vez ya instalada e iniciada la MV de Alpine usamos los siguientes comandos para realizar la configuración de usuario:
  
<img width="572" height="469" alt="image" src="https://github.com/user-attachments/assets/1b714eb0-bad2-40e1-b7c6-7c988b03de9c" />

+ Aqui podemos visualizar la configuración de la interfaz, de usuario y disco, respectivamente ya hecha:
  
<img width="1332" height="866" alt="image" src="https://github.com/user-attachments/assets/22101678-b74d-4edb-bbf0-d74c21f9bf68" />

<img width="1332" height="866" alt="image" src="https://github.com/user-attachments/assets/9cda55cd-776e-4672-a7d1-cdad8e24653e" />

<img width="1332" height="866" alt="image" src="https://github.com/user-attachments/assets/770a944d-3576-4be5-8b05-79edd067ceb1" />

+ Aqui ya se completo toda la instalación:
  
<img width="1332" height="265" alt="image" src="https://github.com/user-attachments/assets/04b5e9af-8f41-46ac-a304-451052d8fed8" />

### Instalacion de Scientific Linux en Maquina Virtual:

+ Se creo manualmente la instalación de Scientific Linux y se creó el disco virtual:
<img width="1600" height="111" alt="image" src="https://github.com/user-attachments/assets/3c4e7198-a946-429d-b615-cb64f563dc26" />

+ Se desplego la pantalla de Scientific Linux y se inicio su instalación:
<img width="653" height="548" alt="image" src="https://github.com/user-attachments/assets/470e6355-3221-4e0d-83d5-ccbf887ddde7" />

+ Iniciamos su configuración conectandolo a la red y demas:
<img width="1297" height="843" alt="image" src="https://github.com/user-attachments/assets/0c821ba0-b98b-4224-b3c2-f73433f11450" />
<img width="1298" height="873" alt="image" src="https://github.com/user-attachments/assets/6423f0a9-133e-43af-9645-9023797e1cd0" />
