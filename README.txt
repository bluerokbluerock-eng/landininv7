LANDINGV7 — INVERSIÓN DIGITAL

Vista local
Abre index.html en el navegador para revisar el diseño. El sitio usa HTML, CSS
y JavaScript sin dependencias de ejecución ni compilación del frontend.

Formulario
Desde esta carpeta, ejecuta node server.mjs con Node 24 y abre
http://localhost:8080. Para registrar solicitudes, copia .env.example a .env,
completa las variables privadas y ejecuta node --env-file=.env server.mjs.

Usa la misma integración con Google Sheets que landininv1. El Apps Script debe
estar desplegado con la versión de sheets-integration/Code.gs que reconoce
landingv7. Usa la URL /exec y el token de ese receptor. Si el envío falla, el
formulario conserva los datos y el identificador para que puedas reintentar.
La pantalla de confirmación aparece cuando el receptor confirma el registro.
La fecha de nacimiento es opcional. El consentimiento es obligatorio.

Railway
Si conectas el repositorio landininv7 a Railway, usa la raíz del repositorio
y /railway.json como archivo de configuración. Si conectas el repositorio
landings, usa /landingv7 como Root Directory y /landingv7/railway.json como
archivo de configuración. Configura GOOGLE_SHEETS_WEBAPP_URL y
GOOGLE_SHEETS_TOKEN como variables del servicio. El Dockerfile ejecuta
Node 24 y escucha en PORT, con 8080 por defecto.

Diseño
Se conservan las secciones, el gráfico ilustrativo, el favicon y la paleta del
ZIP. Los botones verdes usan texto oscuro para mejorar el contraste. Inter
y Manrope se cargan localmente. Las licencias están en assets/licenses/.
