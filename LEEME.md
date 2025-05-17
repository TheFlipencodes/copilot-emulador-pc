<#
    Proyecto: Copilot ia + PC Emulator
    Autor: TheFlipen
    Año: 2025
    Licencia: MIT License
    Descripción: Script principal que emula el Copilot+PC.
#>

# Copilot ia + PC Emulator

Este proyecto busca emular las funcionalidades de **Copilot Plus PC**, originalmente diseñadas para dispositivos Snapdragon Elite y Elite X, pero adaptado para funcionar en cualquier PC con Windows.
Es un conjunto de scripts en PowerShell que emulan funcionalidades similares a Copilot Plus en PCs sin hardware especializado (como NPU).

Automatiza la instalación, ejecución y supervisión del emulador para que funcione continuamente en Windows, monitoreando el estado del sistema (uso de CPU, RAM), gestionando tareas programadas, y generando archivos JSON con información actualizada del estado del emulador. Además, incluye notificaciones para informar al usuario sobre eventos importantes del sistema y del emulador.
Se dedica EXCLUSIVAMENTE mejorar monitorear el rendimiento de tu dispositivo, no tiene orc ni otras funciones 

## Características

- Emulación completa sin necesidad de hardware especializado.  
- Scripts desarrollados principalmente en **PowerShell de Windows** para facilitar su ejecución sin instalaciones adicionales.  
- Uso de notificaciones tipo **toaster** para mostrar mensajes y estados en pantalla de Windows.  
- Compatible con Windows 10 y Windows 11.  
- Pensado para usuarios que no cuentan con hardware Snapdragon pero quieren la experiencia Copilot Plus.

## Scripts del emulador

Este emulador se basa en tres scripts principales y dos opcionales, todos escritos en PowerShell:

1. **Script 1 - Instalador:**  
   Configura el entorno del emulador en el sistema. Crea las carpetas necesarias, instala los scripts y crea la tarea programada para iniciar todo automáticamente al arrancar Windows.

2. **Script 2 - Emulador principal:**  
   Ejecuta la lógica que simula el comportamiento de Copilot Plus PC, monitoreando CPU y RAM, y genera un archivo JSON con el estado del sistema cada 5 segundos.

3. **Script 3 - Supervisor:**  
   Monitorea que el emulador se esté ejecutando correctamente y garantiza su ejecución automática al iniciar Windows.

4. **Script 4 - Notificador (opcional):**  
   Muestra notificaciones tipo toast en Windows (ícono de mensaje a la derecha en la barra de tareas), leyendo el archivo JSON generado por el Script 2 y actualizando la notificación cada 5 segundos.

5. **Script 5 - Verificador integral (opcional):**  
   Comprueba que los scripts clave (Instalador - Script 1, Emulador - Script 2, Supervisor - Script 3, y opcionales 4 y 5) están presentes, si el proceso emulador está corriendo, si la tarea programada supervisor está activa, y muestra el uso actual de CPU y RAM. Además calcula un "estado general" (salud) del sistema basado en esos datos.

> **Nota:**  
> Existió un Script 4 "opcional" que mostraba en pantalla la salida del Script 2, pero quedó obsoleto al crear el Script 5 que reúne y mejora esa funcionalidad.

## Cómo usar

1. Clona este repositorio:  
 
   git clone https://github.com/TheFlipencodes/copilot-emulador-pc.git

    Navega a la carpeta del proyecto y ejecuta los scripts en este orden:

 Script 1,2,3,4,5 siendo el 4 y el 3 opcionales para el proyecto 

Importante: Ejecuta PowerShell como administrador para evitar problemas de permisos y asegurar que los scripts funcionen correctamente.

Licencia

Este proyecto está bajo la licencia MIT. Esto significa que puedes usar, copiar, modificar y distribuir este código libremente, siempre que incluyas la licencia original y atribuyas la autoría a TheFlipen.

Consulta el archivo LICENSE para más detalles.

# Nota sobre IA

Parte del código en este proyecto fue generado con la ayuda de ChatGPT, la inteligencia artificial de OpenAI.

¡Gracias por interesarte en este proyecto y contribuir a mejorar la experiencia Copilot en PCs comunes!



