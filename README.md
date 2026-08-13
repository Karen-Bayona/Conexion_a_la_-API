Guía Paso a Paso para la Configuración y Ejecución
-------------------------------------------------------

Paso a paso para ejecución del codigo.
--------------------------------------------

**Paso 1: Crear y activar el entorno virtual**

- Es necesario aislar el entorno de trabajo para garantizar que se utilicen las versiones correctas de cada librería.

  **En Windows (PowerShell / Símbolo del sistema):**
  
-Control ñ (para abrir la terminal)

-Ejecutar los siguientes comandos

    python -m venv env
  
    .\venv\Scripts\activate
  
Al activarlo correctamente, verás la marca (venv) al inicio de la línea de comandos de tu terminal.

-------------------------------------------------------

**Paso 2: Instalar las dependencias del proyecto**

Con el entorno virtual activo, instala los paquetes requeridos especificados en requirements.txt

    pip install -r requirements.txt

 -------------------------------------------------------

**Paso 3: Configurar la clave de API**

-Obten tu API Key desde Google AI Studio.

-Crea un archivo con el nombre .env en la raíz de tu proyecto (a la altura de los scripts).

-Agrega la siguiente variable dentro del archivo .env:


    GEMINI_API_KEY=tu_clave_api_aqui

 -------------------------------------------------------
 
**Paso 4: Verificar la configuración del entorno**

-Ejecuta el script de diagnóstico para comprobar que estás dentro del entorno virtual y que tu equipo cuenta con salida a Internet:

    python prueba_entorno.py

 -------------------------------------------------------

**Paso 5: Probar la conexión con el Asistente de IA**

Ejecuta el script principal para realizar la solicitud al modelo

    python app_gemini.py
    
Resultado esperado:

🚀 Conectando con el motor de Gemini...

Respuesta Recibida 
¡Hola! Soy un asistente de IA configurado para apoyar el curso de Desarrollo de aplicaciones con IA...

 -------------------------------------------------------

**Imagen de evidencia de la ejecución del script de conexión con respuesta de la API**

<img width="1428" height="334" alt="image" src="https://github.com/user-attachments/assets/49c0f78e-60e7-4856-9e31-a429c53d0abe" />

