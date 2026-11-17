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



#diseño a seguir 
1. Paleta de Colores (Sistema de Diseño)Para transmitir tecnología (IA), confianza (captura de datos) y dinamismo (juegos), usaremos una paleta moderna de alto contraste sobre fondo claro, respetando el wireframe limpio que diseñaste:   Rol en el diseñoColorCódigo HEXUso en Bootstrap 5.3Fondo PrincipalBlanco Humo#F8FAFCFondo general (body) para evitar fatiga visual.Fondo de TarjetasBlanco Puro#FFFFFFContenedores de juegos, pasos y premio.   Color Primario (Marca/IA)Índigo Eléctrico#4F46E5Botones principales ("JUGAR AHORA", "JUGAR"), barras de progreso y acentos IA.   Hover PrimarioÍndigo Oscuro#4338CAEstado al pasar el cursor o tocar un botón.Color Secundario (Premio/Éxito)Esmeralda#10B981Badges de premio, respuestas correctas y validación de formulario.Texto PrincipalPizarra Oscuro#0F172ATítulos (h1, h2) y textos de lectura principal.Texto SecundarioGris Neutro#64748BSubtítulos, textos de apoyo ("Gratis · 1 minuto") y pie de página.   Bordes de TarjetasGris Suave#E2E8F0Contorno de las tarjetas de juego y pasos (border).2. Reglas de Estructura y Componentes (Bootstrap 5.3)Todos los desarrolladores deben usar exactamente estas clases y medidas:Tipografía (Google Fonts): Importar Plus Jakarta Sans (pesos 600 y 700 para títulos y botones) e Inter (pesos 400 y 500 para textos generales).Contenedor Principal (Mobile-First): Como el tráfico viene de celular pero debe verse bien en PC, envuelvan el contenido principal en un contenedor centrado con ancho máximo controlado (max-width: 540px o clase .container ajustada) para que en escritorio parezca una app limpia y no se estire demasiado.Tarjetas (.card):Bordes redondeados: rounded-4 (16px).Borde sutil: border: 2px solid #E2E8F0 (imitando el trazo definido de tu wireframe).   Relleno interno: p-3 o p-4.Botones (.btn):Todos los botones de acción ("JUGAR AHORA", "JUGAR", "ENVIAR") deben llevar: btn btn-primary btn-lg w-100 fw-bold rounded-3 py-3 text-uppercase.   Iconografía: Usar únicamente Bootstrap Icons (bi-lock, bi-shield-check, bi-clock, etc.) para que los íconos de confianza y las interfaces de ambos juegos tengan el mismo grosor de línea.   
