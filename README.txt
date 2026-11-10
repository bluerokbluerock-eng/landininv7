LANDINGV7 — INVERSIÓN DIGITAL

Vista local
Abre index.html en el navegador para revisar el diseño. El sitio usa HTML, CSS
y JavaScript sin dependencias de ejecución ni compilación del frontend.

Formulario
Desde esta carpeta, ejecuta node server.mjs con Node 24 y abre
http://localhost:8080. Para registrar solicitudes, copia .env.example a .env,
completa las variables privadas y ejecuta node --env-file=.env server.mjs.

CRM_BACKEND_URL es la URL del servicio crm-api (por ejemplo, http://localhost:3000).
El servidor envía el formulario a POST /api/v1/leads/landingv7 con la clave
privada CRM_LANDING_V7_API_KEY, que debe coincidir en ambos servicios. El CRM
asigna los registros al área Sale (2), la campaña 25 y el estado 31.
Los registros aparecen en Leads Metrics según los permisos del CRM.
Si falla el envío, el formulario conserva los datos y el
identificador para el reintento. Solo muestra confirmación si el CRM registra
la solicitud. La fecha de nacimiento es opcional y el consentimiento es obligatorio.

Railway
Si conectas el repositorio landininv7 a Railway, usa la raíz del repositorio
y /railway.json como archivo de configuración. Si conectas el repositorio
landings, usa /landingv7 como Root Directory y /landingv7/railway.json como
archivo de configuración. Configura CRM_BACKEND_URL y
CRM_LANDING_V7_API_KEY como variables del servicio. El Dockerfile ejecuta
Node 24 y escucha en PORT, con 8080 por defecto.

Diseño
Se conservan las secciones, el gráfico ilustrativo, el favicon y la paleta del
ZIP. Los botones verdes usan texto oscuro para mejorar el contraste. Inter
y Manrope se cargan localmente. Las licencias están en assets/licenses/.
