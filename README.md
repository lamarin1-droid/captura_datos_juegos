# captura_datos_juegos
Utilizando IA el cliente necesita un sitio web con 2 juegos que puedan jugar en linea con el objetivo de atraer gente y capturar sus datos , ese como objetivo principal , el juego es solo un distractor

Requerimientos Funcionales (RF)
1. Captura de Datos y Conversión (Objetivo Principal)
RF-01 (Formulario de registro): Solicitar datos básicos (nombre, correo y teléfono) antes de iniciar o al finalizar la partida para desbloquear el puntaje o premio.

RF-02 (Validación y exportación): Verificar que el correo sea real, evitar registros duplicados y permitir descargar la base de datos en Excel/CSV.

2. Juegos Web e Integración de IA (Distractor)
RF-03 (Ejecución directa de 2 juegos): Permitir jugar ambos minijuegos directamente en el navegador sin descargar aplicaciones externas.

RF-04 (Dinamismo con IA): Utilizar IA para personalizar la partida (ej. generar preguntas dinámicas o un perfil de resultado personalizado) que motive al usuario a dejar sus datos.

Requerimientos No Funcionales (RNF)
1. Rendimiento y Usabilidad Móvil
RNF-01 (Diseño Mobile-First): Los juegos y el formulario deben adaptarse 100% a pantallas táctiles de celular, de donde proviene la mayoría del tráfico.

RNF-02 (Velocidad de carga): La página y las respuestas de la IA deben cargar en menos de 3 segundos para evitar que el usuario abandone antes de registrarse.

2. Seguridad y Privacidad
RNF-03 (Protección de datos): Incluir casilla de aceptación de políticas de privacidad (cumplimiento LOPDP) y certificado de seguridad HTTPS.

RNF-04 (Protección de API y anti-bots): Ocultar las claves de la IA en el servidor (backend) y bloquear registros automatizados o puntajes falsos.
