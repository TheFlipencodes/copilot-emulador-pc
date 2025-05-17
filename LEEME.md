# copilot-emulador-pc
## Licencia

Este proyecto está bajo la licencia GPL v3. Consulta el archivo LICENSE para más detalles.

emula Copilot + Pc con powershell
# Copilot Plus PC Emulator

Este proyecto busca emular las funcionalidades de **Copilot Plus PC** originalmente diseñadas para dispositivos con procesador Snapdragon Elite y Elite X , pero adaptado para funcionar en cualquier PC con Windows.

## Características
- Emulación completa sin necesidad de hardware especializado.
- Scripts desarrollados principalmente en **PowerShell de Windows** para facilitar su ejecución sin instalaciones adicionales.
- Uso de notificaciones tipo **toaster** para mostrar mensajes y estados en pantalla de windows .
- Compatible con Windows 10 y Windows 11.
- Pensado para usuarios que no cuentan con hardware Snapdragon pero quieren la experiencia Copilot Plus.

# Copilot Plus PC Emulator

Este proyecto busca emular las funcionalidades de **Copilot Plus PC** originalmente diseñadas para dispositivos Snapdragon, pero adaptado para funcionar en cualquier PC con Windows.

## Cómo usar

Este emulador se basa en tres scripts principales escritos en PowerShell:

1. **Instalador**: Configura el entorno del emulador en el sistema. Script 1 - Instalador para el emulador Copilot Plus PC, que configura la carpeta, instala el script 2 (emulador), y crea la tarea programada para que todo se inicie automáticamente al arrancar Windows:
2. **Emulador principal**: Ejecuta la lógica que simula el comportamiento de Copilot Plus PC.
3. **Supervisor**: Monitorea el emulador y garantiza su ejecución automática al iniciar Windows.

### Pasos:

1. Clona este repositorio:  
   ```bash
   git clone https://github.com/TheFlipencodes/copilot-emulador-pc.git
   
## Nota sobre IA

Parte del código en este proyecto fue generado con la ayuda de **ChatGPT**, la inteligencia artificial de OpenAI.


