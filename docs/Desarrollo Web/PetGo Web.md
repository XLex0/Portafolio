# PetGo Web


<p>
  <img src="https://img.shields.io/badge/Azure%20DevOps-0078D7?style=for-the-badge&logo=azuredevops&logoColor=white"/>
  <img src="https://img.shields.io/badge/SonarCloud-F3702A?style=for-the-badge&logo=sonarcloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jakarta%20EE-E95420?style=for-the-badge&logo=java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white"/>
  <img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white"/>
</p>

## Colaboradores

Proyecto realizado por:  
<b>Jefferson Chileno</b>  
<b>Pablo Maldonado</b>  
<b>Emilio Quinga</b>  
<b>Alexander Motoche</b> <sub><i>(Líder proyecto)</i></sub>


### Descripción:
PetGo es una aplicación web que conecta a dueños de mascotas con paseadores de perros disponibles en su zona.  
Su objetivo es facilitar el proceso de búsqueda y emparejamiento entre ambas partes.

### Resultados
<p>En las siguientes imágenes se muestran las principales interfaces y resultados del sistema:</p>

<div style="width:100%; max-width:600px; margin:auto; position:relative;">
  <!-- Marco del slider: altura fija y fondo para que no “salte” -->
  <div id="slider"
       style="
        width:100%;
        height:360px;              /* <- controla la altura del cuadro */
        background:#0b0b0b;        /* fondo neutro detrás de la imagen */
        overflow:hidden;
        position:relative;
        border-radius:12px;
       ">
    <!-- Todas las imágenes ocupan el mismo cuadro -->
    <img src="../../images/Pg1.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:block;"/>
    <img src="../../images/Pg2.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg3.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg4.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg5.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg7.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg8.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg9.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg10.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg11.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
    <img src="../../images/Pg12.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none;"/>
  </div>

  <!-- Botones bonitos -->
  <button onclick="moveSlide(-1)"
    style="position:absolute; top:50%; left:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;
           transition:.2s;">❮</button>

  <button onclick="moveSlide(1)"
    style="position:absolute; top:50%; right:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;
           transition:.2s;">❯</button>
</div>

<script>
let current = 0;
const imgs = document.querySelectorAll("#slider img");
function moveSlide(n){
  imgs[current].style.display = "none";
  current = (current + n + imgs.length) % imgs.length;
  imgs[current].style.display = "block";
}
</script>


### Gestión del Proyecto
Para el desarrollo de PetGo Web, se aplicó la metodología Scrum utilizando Azure DevOps como herramienta principal de gestión.
El equipo trabajó en sprints donde se definieron y priorizaron user stories y tasks en el backlog.
Cada sprint incluía:

Sprint Planning: Definición del alcance y estimación de tareas.

Daily Meetings: Seguimiento del progreso y resolución de bloqueos.

Sprint Review y Retrospective: Evaluación de los entregables y mejora continua del proceso.

<div style="width:100%; max-width:600px; margin:auto; position:relative;">
  <div id="slider2"
       style="width:100%; height:360px; background:#0b0b0b; overflow:hidden; position:relative; border-radius:12px;">
    <img src="../../images/PgG1.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:block; transition:opacity .3s;"/>
    <img src="../../images/PgG2.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgG3.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgG4.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgG5.png"  style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
  </div>

  <button onclick="moveSlide2(-1)"
    style="position:absolute; top:50%; left:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;">❮</button>

  <button onclick="moveSlide2(1)"
    style="position:absolute; top:50%; right:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;">❯</button>
</div>

<script>
let current2 = 0;
const imgs2 = document.querySelectorAll("#slider2 img");

function moveSlide2(n) {
  imgs2[current2].style.display = "none";
  current2 = (current2 + n + imgs2.length) % imgs2.length;
  imgs2[current2].style.display = "block";
}
</script>

### Integración y Despliegue Continuo
Durante el desarrollo del proyecto PetGo Web, utilizamos Azure DevOps no solo como herramienta de gestión ágil, sino también como la plataforma principal para implementar Integración Continua (CI) y Despliegue Continuo (CD).

Dentro del pipeline de integración, se incorporó SonarCloud como herramienta de análisis estático de código
<div style="width:100%; max-width:600px; margin:auto; position:relative;">
  <div id="slider3"
       style="width:100%; height:360px; background:#0b0b0b; overflow:hidden; position:relative; border-radius:12px;">
       
    <img src="../../images/PgCI1.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:block; transition:opacity .3s;"/>
    <img src="../../images/PgCI2.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgCI3.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgCI4.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>
    <img src="../../images/PgCI5.png" style="position:absolute; inset:0; width:100%; height:100%; object-fit:contain; display:none; transition:opacity .3s;"/>

  </div>

  <!-- Botones -->
  <button onclick="moveSlide3(-1)"
    style="position:absolute; top:50%; left:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;">❮</button>

  <button onclick="moveSlide3(1)"
    style="position:absolute; top:50%; right:10px; transform:translateY(-50%);
           background-color:rgba(0,0,0,0.45); border:none; color:#fff;
           font-size:22px; padding:8px 12px; border-radius:50%; cursor:pointer;">❯</button>
</div>

<script>
let current3 = 0;
const imgs3 = document.querySelectorAll("#slider3 img");

function moveSlide3(n) {
  imgs3[current3].style.display = "none";
  current3 = (current3 + n + imgs3.length) % imgs3.length;
  imgs3[current3].style.display = "block";
}
</script>

### Código y Arquitectura
El desarrollo de PetGo Web se realizó utilizando el lenguaje Java, bajo el framework Jakarta EE, siguiendo una estructura modular basada en componentes y controladores.
El proyecto fue configurado como un archivo Maven, lo que permitió gestionar dependencias, empaquetar el proyecto eficientemente y mantener la compatibilidad con los entornos de integración y despliegue continuo en Azure DevOps.

<p>
  📘 Para más detalles sobre la arquitectura y diseño, consulta el  
  <a href="../../resources/ManualTecnicoPetGo.pdf" target="_blank"><b>Manual Técnico</b></a>.
</p>

<p>
  🌐 También puedes explorar el proyecto completo en  
  <a href="https://dev.azure.com/Xelan/GR06-ISWD622-25A" target="_blank"><b>Azure DevOps</b></a>.
</p>
