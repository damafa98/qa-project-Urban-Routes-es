## Proyecto Urban Routes

Daniela Malagon, Sprint 8

##Descripción

Este proyecto automatiza pruebas funcionales para la aplicación Urban Routes utilizando Python, Selenium y Pytest bajo el patrón Page Object Model (POM). El objetivo es cubrir el flujo completo para solicitar un taxi en la aplicación, asegurando que cada paso funcione correctamente y que la experiencia del usuario sea estable y confiable.

Se desarrollaron localizadores, métodos y pruebas automatizadas que simulan el proceso real de un usuario. Todas las pruebas fueron ejecutadas en PyCharm, y se utilizó el archivo data.py para gestionar la configuración y los datos de prueba, incluyendo la URL del servidor, que debe actualizarse antes de cada ejecución.

##Requisitos
- Selenium
- Python
- pytest
- Servidor de Urban Routes

##Instalación
1. Instala Python
    Descárgalo desde python.org e instálalo en tu sistema.
2. Clona el repositorio:
   git clone <URL-del-repositorio>
   cd <nombre-del-repositorio>
3. Instala dependencias (Ejecuta en la terminal):
   pip install selenium pytest requests
4. Instala ChromeDriver
   Descárgalo desde chromedriver.chromium.org
   Asegúrate de que esté en tu PATH o en el directorio del proyecto.
5. Configura la URL del servidor
    Abre data.py y actualiza la variable urban_routes_url con la URL activa del servidor, por ejemplo:
    urban_routes_url = "https://cnt-35bd9ac8-d7a6-43a8-a508-444759dd0ac3.containerhub.tripleten-services.com?lng=es"

##Pruebas Automatizadas Incluidas
1. Configurar la dirección
2. Seleccionar la tarifa Comfort
3. Rellenar el número de teléfono
4. Agregar una tarjeta de crédito
5. Escribir un mensaje para el conductor 
6. Pedir una manta y pañuelos
7. Pedir 2 helados 
8. Aparece el modal para buscar un taxi
9. Esperar a que aparezca la información del conductor en el modal

##Instrucciones para Ejecutar las Pruebas
1. Verifica que la URL del servidor en data.py esté actualizada y activa.
2. Asegúrate de que ChromeDriver esté instalado y accesible. 
3. Abre una terminal en la carpeta raíz del proyecto. 
4. Ejecuta el siguiente comando para correr todas las pruebas:
   pytest main.py
   #Si tus pruebas están en una carpeta específica, usa:
     pytest ruta/a/tu/test_file.py
   #Para ver resultados detallados, agrega la opción -v:
     pytest -v main.py

##Consideraciones Finales
- Si la aplicación web cambia de estructura o idioma, revisa y actualiza los selectores y valores esperados en los asserts.
- Si alguna prueba falla, revisa los mensajes de error y asegúrate de que los datos de prueba sean válidos y la URL del servidor esté disponible. 
- Se recomienda verificar otras funcionalidades no cubiertas antes de lanzar la aplicación a producción.