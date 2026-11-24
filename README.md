<h1 align="center">Mar Agramonte</h1>

<p align="center">
  <b>QA Automation y Backend Java</b><br>
  Spring Boot · PostgreSQL · Docker · Playwright · Testing de APIs · 400 h de QA en Marlink<br>
  Palma de Mallorca · Presencial o híbrido, remoto o reubicación · Incorporación inmediata
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/maragramonte/"><img src="https://img.shields.io/badge/LinkedIn-Ver_perfil-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Ver perfil de LinkedIn"></a>
  <a href="mailto:agramontecampos01@gmail.com"><img src="https://img.shields.io/badge/Email-Escríbeme-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Enviar un email"></a>
  <a href="https://maragramonte.com/"><img src="https://img.shields.io/badge/Portfolio-Ver_proyectos-176B5B?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Visitar mi portfolio"></a>
  <a href="https://forms.gle/dUs98Lvra13gpzT97"><img src="https://img.shields.io/badge/CV-Pídemelo-374151?style=for-the-badge&logo=readdotcv&logoColor=white" alt="Pedir mi CV con un formulario"></a>
</p>

## Del mostrador al backend

Dos pacientes intentan reservar la misma hora a la vez. Solo uno la consigue y el otro recibe un aviso claro. Eso lo programé yo y lo probé contra una base de datos real.

Vengo de la administración, la recepción y la atención al cliente, y me titulé en DAM en CESUR Mallorca (2024–2026). Se nota cuando programo: lo primero que pienso es quién va a usar esto y qué se le puede romper.

Busco mi primer puesto como QA Automation o desarrolladora backend con Java 21 y Spring Boot. Dejo cada decisión técnica por escrito, con la alternativa que descarté. Uso la IA a diario, pero nada de lo que propone entra sin pruebas.

## Proyectos

### [Dr. Agramonte](https://github.com/maragramonte/dr-agramonte)

<p align="center"><a href="https://demo-dragramonte.maragramonte.com/"><img src="assets/projects/dr-agramonte.jpg" alt="Página de inicio y agenda de reservas de Dr. Agramonte" width="900"></a></p>

App de citas para un internista de Palma. Los pacientes reservan, cambian y cancelan su cita desde el móvil, sin llamar. Backend con Java 21, Spring Boot 3.5, PostgreSQL, JWT y Flyway. El bloqueo pesimista en PostgreSQL evita las reservas dobles, y una prueba de concurrencia lo demuestra.

- 138 pruebas de backend (unitarias, de API y con Testcontainers) y 47 E2E con Playwright, con axe-core para la accesibilidad.
- CI con GitHub Actions en cada push.
- Revisor de pull requests en Python que usa la API de Claude, con 15 pruebas propias. Se activa con una clave de API.
- [Demo](https://demo-dragramonte.maragramonte.com/), con datos ficticios.

### [Photo Palette](https://github.com/maragramonte/photo-palette)

<p align="center"><a href="https://paleta.maragramonte.com/"><img src="assets/projects/photo-palette.jpg" alt="Portada de Photo Palette: la foto de un eclipse con una regla de color que mide lo que ocupa cada tono, y debajo sus colores vivos" width="900"></a></p>

Le das una foto y te devuelve sus colores principales, listos para una web: HEX, RGB, porcentaje y un bloque `:root` para copiar. Java 21 y Spring Boot 3.5, con k-means escrito a mano. La foto se analiza en memoria y no se guarda. Nació de mis fotos del cielo de noche: quería sacar sus colores.

- Modo `vivos`: ignora sombras y ruido y ordena por saturación, para no perder el color por el que hiciste la foto.
- Límites por IP con Bucket4j, semáforo de análisis y errores en ProblemDetail.
- 98 pruebas, con un 97 % de cobertura de líneas. JaCoCo pone un suelo de cobertura en el CI.
- 21 E2E de la web con Playwright, en escritorio y móvil, con axe-core.
- Imagen Docker en GHCR, web en GitHub Pages y API en Render.
- [Pruébala con una foto tuya](https://paleta.maragramonte.com/)

### [Farmacia Agramonte](https://github.com/maragramonte/Farmacia-Agramonte)

<p align="center"><a href="https://farmacia.maragramonte.com/"><img src="assets/projects/farmacia-agramonte.jpg" alt="Página principal de Farmacia Agramonte" width="900"></a></p>

La web de una farmacia de barrio real de El Born, en Barcelona. Los clientes ven el catálogo y mandan su encargo por WhatsApp, en castellano, catalán o inglés. Sin cookies ni frameworks.

- No quería mantener 154 páginas a mano: un generador en Python crea 143 a partir de dos JSON.
- El catálogo se importa del CSV del programa de gestión.
- 218 tests de pytest vigilan el generador, el importador y los enlaces.
- [Web](https://farmacia.maragramonte.com/)

### [Mi portfolio](https://github.com/maragramonte/mi-portfolio)

Mi portfolio con React y Vite, en español e inglés, con tema de día y de noche.

- 59 pruebas E2E en un Chrome real: idioma, tema, navegación, filtros, menú del móvil y accesibilidad con axe-core.
- En GitHub Actions corren en cada pull request y antes de cada despliegue. Si falla una, no se publica.
- [Web](https://maragramonte.com/)

### [Proyectos de clase](https://github.com/maragramonte/proyectos-dam)

Una selección de lo que hice en DAM: tres simulaciones de concurrencia en Java, con hilos, semáforos y sockets, y una app Android de tareas en Kotlin con SQLite.

## Experiencia

**Marlink Group (OmniAccess) · Prácticas de desarrollo y QA** · ene–mar 2026 · 400 h · Parc Bit, Palma  
- Pruebas funcionales de la API de Ucopia: diseño de casos, reproducción de fallos e informes en Jira.
- Validación de flujos E2E en entornos simulados y de producción.
- Scripts en Python para consultar SQL y MongoDB desde Docker sobre WSL.
- Equipo ágil con SAFe (Daily, Sprint Planning y PI Planning) y documentación en Confluence.

**GladToLink · Prácticas de consultoría tecnológica** · feb 2025 · 100 h  
Formularios y maquetación en XML, gestión documental con Adobe y Java para botones e interacciones, en proyectos de digitalización.

**Antes de IT**  
Cajera en El Corte Inglés (2025), recepción de las salas VIP del aeropuerto de Palma (2024) y un año en The Ardilaun Hotel de Galway, Irlanda, trabajando en inglés (2023–2024). Antes, prácticas de administración y RRHH en Urbia Servicios Integrales y atención al cliente en Natural World Eco (2021). De allí me traje la calma cuando hay prisa.

## Stack

![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=springboot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?logo=spring&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?logo=flyway&logoColor=white) ![JUnit](https://img.shields.io/badge/JUnit-25A162?logo=junit5&logoColor=white) ![Testcontainers](https://img.shields.io/badge/Testcontainers-25A162?logo=testcontainers&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![React](https://img.shields.io/badge/React-149ECA?logo=react&logoColor=white)

También trabajo con SQL, MySQL, MongoDB, SQLite, APIs REST, JavaScript, HTML, CSS, XML, Git, Linux, WSL, Docker Compose, DBeaver y Odoo. Conozco Scrum, Kanban y SAFe; he utilizado Jira y Confluence.

## Formación e idiomas

- **Técnica Superior en Desarrollo de Aplicaciones Multiplataforma (DAM)** · CESUR Mallorca · 2024–2026
- Español y catalán: nativos · Inglés: B2 (un año trabajando en Irlanda)
