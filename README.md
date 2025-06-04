## Proyecto Urban Routes 
# Pruebas automatizadas con Selenium para la verificacion de las funciones de Urban Routes con Python
Daniela Malagon, Sprint 8
## Descripción


Se realizó el siguiente archivo en Pycharm utilizando todo lo anteriormente aprendido y estudiado, se realizaron las pruebas con ayuda de Pytest  y Selenium, mas especificamente se utilizó el metodo POM (Page Object Model) . Primero realicé la definición de los localizadores, luego se crearon los métodos requeridos y al final ya se pudieron ejecutar las pruebas. Las pruebas que se realizarón debían cubrir el proceso completo para pedir un taxi en la aplicación.

NOTA: Antes de ejecutar las pruebas, debemos actualizar la URL del servidor, esta es necesita refrescarse. Actualizas la url copiandolo en data, modificas la variable urban_routes_url actualizando entre '', la nueva URL.

## Requisitos

- Selenium
- Python
- pytest
- Servidor de Urban Routes

## Instalaciones

1. Descarga de python
2. Descarga de Pytest desde PyCharm
3. Descarga de Github
4. Descarga de paquete selenium, desde el comando pip install
5. Descarga de paquete request, desde el comando pip install
5. Clonar el repositorio
6. Instalación de ChromeDriver

## Contenido

El proyecto contine 6 carpetas, el las cuales se encuentra:
1. data.py: Dentro de este se almacena la información que se enviara en las solicitudes, así mismo las configuraciones para el proyecto en donde se almacenan la ruta al servidor.
2. main.py: Dentro de este se encuentra las pruebas para realizar el pedido del taxi.
3. Pages.py: Dentro de esta se encuentran los localizadores de las funciones relacionadas con las distintas páginas de tu aplicación
4. helpers.py: En esta se encuentra la funcionalidad retrieve_phone_code, el cual devuelve un número de confirmación de teléfono
5. README.md: El cual guarda la descripción del proyecto.
6. gitignore: En este se guardan archivos para que Git los descarte

  **A continuación se detallan las pruebas realizadas:**

    1. **Configurar la dirección**
       
  
    2. **Seleccionar la tarifa Comfort.**
     
  
    3. **Rellenar el número de teléfono.**
    
  
    4. **Agregar una tarjeta de crédito**
      
  
    5. **Escribir un mensaje para el controlador.**
       
  
    6. **Pedir una manta y pañuelos**
       
  
    7. **Pedir 2 helados.**
       
  
    8. **Aparece el modal para buscar un taxi.**
      
  
    9. **Esperar a que aparezca la información del conductor en el modal **


 ## Conclusiones

 La aplicacion presenta una pagina estable, las pruebas fueron existosas en los requerimientos solicitados para el trabajo. Se recomienda verificar las siguientes opciones no probadas antes de lanzar la aplicacion para el publico para confirmar que no haya una fallo no revisado en estos pasos.
