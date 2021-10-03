<template>
  <div>
    <div class="row justify-content-center">
      <div class="col-md-4">
        <img src="/img/imgfront.png" width="100%" />
      </div>
      <div class="col-md-6 pt-5">
        <div class="row justify-content-center">
          <h1>Cursos virtuales para profesores</h1>
          <ul>
            <li>
              <h3 class="mt-3">
                Ahora puedes dominar todas las herramientas para poder enseñar
                virtualmente en un 100%
              </h3>
            </li>
            <li>
              <h3 class="mt-3">
                Certificación validada por el organismo del estado
              </h3>
            </li>
            <li>
              <h3 class="mt-3">Estudia a tu rítmo en tus tiempos libres</h3>
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="row justify-content-center">
          <h3>
            Clases
          </h3>
        </div>
        <div class="row justify-content-center">
          <p>
            Toma clases rápidas y prácticas en tus ratos libres
          </p>
        </div>
        <div class="row justify-content-center">
          <div class="col-md-3">
            <b-card
              title="Google ClassRoom"
              img-src="/img/classroom.jpg"
              img-alt="Image"
              img-top
              tag="article"
              style="max-width: 20rem;"
              class="mb-2"
            >
              <b-card-text>
                Aprende como crear, agregar, calificar tareas para llevar tus
                clases virtuales.
              </b-card-text>

              <b-button to="/cursos/1/1" variant="primary"
                >Tomar Clases</b-button
              >
            </b-card>
          </div>
          <div class="col-md-3">
            <b-card
              title="Google Meet"
              img-src="/img/googlemeet.png"
              img-alt="Image"
              img-top
              tag="article"
              style="max-width: 20rem;"
              class="mb-2"
            >
              <b-card-text>
                Aprende a crear reuniones, programar, invitarlas y usar todas
                sus herramientas.
              </b-card-text>

              <b-button to="/cursos/2/1" variant="primary"
                >Tomar Clases</b-button
              >
            </b-card>
          </div>
          <div class="col-md-3">
            <b-card
              title="Zoom"
              img-src="/img/zoom.png"
              img-alt="Image"
              img-top
              tag="article"
              style="max-width: 20rem;"
              class="mb-2"
            >
              <b-card-text>
                Aprende a crear reuniones, programar, invitarlas y usar todas
                sus herramientas.
              </b-card-text>

              <b-button to="/cursos/3/1" variant="primary"
                >Tomar Clases</b-button
              >
            </b-card>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md-12">
        <div class="row justify-content-center mt-5">
          <h3>
            Foro
          </h3>
        </div>
        <div class="row justify-content-center">
          <div class="col-md-5 foro-item">
            <div class="row">
              <div class="col-md-9">
                <div class="row">
                  <b>2 de Octubre del 2021</b>
                </div>
                <div class="row">
                  <h3>¿Cómo calificar automaticamente un examen?</h3>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-5 foro-item">
            <div class="row">
              <div class="col-md-9">
                <div class="row">
                  <b>2 de Octubre del 2021</b>
                </div>
                <div class="row">
                  <h3>¿Cómo puedo compartir archivos con mis alumnos en google drive?</h3>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-md-5 foro-item">
            <div class="row">
              <div class="col-md-9">
                <div class="row">
                  <b>2 de Octubre del 2021</b>
                </div>
                <div class="row">
                  <h3>¿Cómo calificar automaticamente un examen?</h3>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-5 foro-item">
            <div class="row">
              <div class="col-md-9">
                <div class="row">
                  <b>2 de Octubre del 2021</b>
                </div>
                <div class="row">
                  <h3>¿Cómo calificar automaticamente un examen?</h3>
                </div>
              </div>
            </div>
          </div>
        </div>
     
        
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.card {
  color: #000000;
}
.foro-item {
  background-color: #4262b9;
  padding: 10px;
  border-radius: 20px;
  margin: 10px;
}
</style>
