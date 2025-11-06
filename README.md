# 1.0 Inicio

Este repositorio es acerca de una app hecha con Spring Boot, dictada por el profesor [Daniel Felipe Agudelo Molina](https://github.com/DanielDev87)
Este es el backend de una app para crear vehículos; puedes consultar el Front [aquí](https://github.com/DavidMrn/leng-app-vehiculos-front) 
## ⚠️ 1.1 Requisitos

- JDK 17 o superior. Puedes instalarlo aquí
- Visual Studio Code
- [Postman](https://www.postman.com/downloads/) (Descargar) 
## 📦 1.2 Extensiones

- [Extension Pack For Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)
- [Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=vmware.vscode-boot-dev-pack)

# 2.0 Funcionamiento

Lo primero que se realiza es la descarga de los archivos del repositorio; para eso puedes ir a el botón verde **"<>Code"** y descargar el **.Zip**
También puedes clonarlo con [Git](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository). 

Los métodos serán enviados mediante Postman el cual permite un mejor uso de imágenes.

Para usarlo deberás irte a Postman tus espacios de trabajo (Workspaces) y crear una nueva request mediante el boton **+**

## 2.1 Todas las rutas de la App.

### 2.2 Vehículos

**Crear Vehículo**: Para crear uno usamos la ruta `http://localhost:8080/api/vehiculos` y ponemos los atributos en el body.
Como vamos a enviar debemos usar el método **POST**. 

Puedes seguir este ejemplo: {"marca":"Lexus","modelo":"Ls400","anio":1994}

<img width="1477" height="541" alt="Crearvehiculo" src="https://github.com/user-attachments/assets/cf3d1cbc-10fd-43a8-8dea-8590bda5e7d4" />


**Obtener Vehiculos:** Consultar todos los vehículos (y ver su ruta)
`http://localhost:8080/api/vehiculos` 
Como vamos a consultar información cambiamos el método por **GET**

<img width="1477" height="638" alt="Obtenertodosvehiculos" src="https://github.com/user-attachments/assets/27aaddf1-f06a-4a17-83b8-bf6277abe437" />


**Obtener Vehículo Por ID:** Especificamos que id o vehículo queremos que nos muestre.
`http://localhost:8080/api/vehiculos/2` 
También se usa **GET**.

<img width="1477" height="489" alt="Obtenervehiculoporid" src="https://github.com/user-attachments/assets/581abc39-4c00-4489-8eb1-7241ca906c02" />


**Editar Vehículo:** Para editar el vehículo, sus características e imagen. (Usando el ID)
`http://localhost:8080/api/vehiculos/1`
Usamos el método **PUT**.
En este ejemplo solo cambié las mayúsculas por minúsculas (Ten en cuenta que puedes modificar todo)

<img width="1480" height="553" alt="editarvehiculo" src="https://github.com/user-attachments/assets/911c144d-4bbf-4e8b-837b-0a5e9d21534a" />


**Eliminar Vehículo:** Mediante su ID y utilizando el método **DELETE**

<img width="1479" height="383" alt="eliminarvehiculo" src="https://github.com/user-attachments/assets/4ed5eb99-2f37-41e9-95c3-0c7f8a51787b" />


---

### 2.3 Motos

**Crear Moto**: Para crear moto usamos la ruta: `http://localhost:8080/api/motos` con el método **POST**, ya que vamos a crear o enviar. De igual manera, si queremos consultar las motos más adelante cambiamos el método a **GET** y no enviamos body.


Puedes seguir este ejemplo:
{"marca": "Ducati", "modelo": "Panigale V4 S", "anio": 2024}

<img width="1475" height="534" alt="crearmoto" src="https://github.com/user-attachments/assets/29ca5d51-4b31-4329-a9a5-d239bd87c586" />


**Obtener Moto Por ID:** Con la ruta `http://localhost:8080/api/motos/3`
Obtendremos la moto con el ID número 3. 

<img width="1480" height="524" alt="obtenermotoporid" src="https://github.com/user-attachments/assets/101f3b1e-cb05-45bf-9510-fc85e81dbeb7" />


**Editar Moto:** 

Para editar el vehículo, sus características e imagen. (Usando el ID)
`http://localhost:8080/api/motos/3`
Usamos el método **PUT**.


**Eliminar Moto**: Así como el de vehiculos, mediante su ID y método **DELETE** con la ruta de ejemplo: `http://localhost:8080/api/motos/3`
