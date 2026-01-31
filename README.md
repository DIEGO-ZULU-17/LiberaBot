📂 Documentación del Proyecto: LiberaBot https://diegozulu17.app.n8n.cloud/workflow/myMp9mMYIZXwNpIfJSQiC

🎯 1. Objetivo del Proyecto

Desarrollar un asistente virtual inteligente en Telegram que ayude a los usuarios a alcanzar la libertad financiera. El bot facilita el registro inmediato de ingresos y gastos, eliminando la fricción de las hojas de cálculo manuales, y utiliza Inteligencia Artificial para motivar al usuario, generar imágenes inspiradoras y actuar como un asesor financiero que analiza los datos para sugerir estrategias de inversión (Bolsa de Valores).

🧩 2. Problema que Resuelve

    Falta de disciplina en el registro: La mayoría de las personas abandonan sus presupuestos porque es tedioso abrir Excel diariamente. El bot permite hacerlo como si chatearas con un amigo.
    Ausencia de análisis: Registrar datos no sirve si no se interpretan. El bot no solo guarda números, sino que calcula balances y ofrece consejos personalizados mediante IA.
    Falta de motivación: El ahorro suele verse como una restricción. LiberaBot lo convierte en una experiencia positiva enviando frases motivadoras e imágenes generadas por IA tras cada registro.
    Limitación técnica de automatizaciones simples: Resuelve el problema de los bots "sin memoria" implementando una Máquina de Estados en Google Sheets, permitiendo conversaciones fluidas paso a paso sin perder el hilo.

🔄 3. Cómo se Usa (Flujo del Usuario)

El usuario interactúa con el bot en Telegram mediante botones y texto. El flujo es cíclico:

    Inicio: El usuario envía "Hola" o "/start".
    Menú Principal: El bot responde con botones: (1) Registrar Transacción o (2) Ver Reporte.
    Opción A - Registro: El usuario selecciona Ingreso o Gasto. Posteriormente, elige una Categoría predefinida según el tipo de transacción:

    Si es Ingreso: [Salario], [Venta], [Regalo].
    Si es Gasto: [Vivir], [Diversión], [Ahorro], [Caridad], [Educación], [Inversiones].

Luego, escribe el Concepto (ej. "Cena con amigos") y el Monto (ej. "50000").

Resultado: El bot guarda los datos en Google Sheets, confirma el registro exitoso y envía una imagen y frase motivacional única generada por IA.

    Opción B - Reporte:

El bot lee todos los registros históricos.

Calcula Ingresos vs. Gastos.

Resultado: Envía un análisis detallado hecho por IA con consejos para mejorar las finanzas.

🛠️ 4. Herramientas y Stack Tecnológico

Este proyecto desarrollado en n8n utiliza las siguientes tecnologías:

    n8n (Workflow Automation): Orquestador central. Maneja la lógica, los condicionales (Switch/If) y la conexión entre servicios.
    Telegram Bot API: Interfaz de usuario (Chat, Botones Inline, envío de fotos).
    Google Sheets (Base de Datos):
        Hoja "Datos": Almacena el historial financiero (Fecha, Monto, Concepto, etc.).
        Hoja "UserStates": Funciona como memoria temporal para saber en qué paso de la conversación está cada usuario.
    Google Gemini (Inteligencia Artificial):
        Modelo de Chat: Para generar frases motivadoras y el análisis financiero del reporte.
        Modelo de Visión/Imagen: Para generar las imágenes de "Libertad Financiera".

🔗 5. Recursos del Proyecto

Aquí están los enlaces y credenciales (simuladas/públicas) que has utilizado para la configuración:

    Estructura de Base de Datos (Google Sheets):
        https://docs.google.com/spreadsheets/d/1je3W-2TGt_czvbHrOe92NQUWRS26WXZknIcIhu2Qp0M/edit?usp=sharing
        Nota: Contiene las pestañas Datos y UserStates.
    Plataforma de Automatización:
        https://diegozulu17.app.n8n.cloud/workflow/myMp9mMYIZXwNpIfJSQiC
    Canal de Interacción:
        Bot de Telegram (Configurado previamente con BotFather): 8519618752:AAEA0SlfYgz8oblem75PBgXL-5GUgvtUAFA.
        API Google: AIzaSyBhgmG7EDlJmUaWuwyAgCqfM1qMfwgpvn8

