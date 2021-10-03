<template>
  <div class="content-class">
    <div class="row">
      <div class="col-md-9">
        <div class="row">
          <h3>{{ video.number }} ) {{ video.title }}</h3>
        </div>
        <div class="row">
          <video-player :src="video.url" />
        </div>
      </div>
      <div class="col-md-3">
        <h4>{{ course.title }}</h4>
        <ol>
          <li v-for="item in videos">
            <NuxtLink :to="item.url">{{ item.title }}</NuxtLink>
          </li>
        </ol>
      </div>
    </div>
    <div class="row">
      chat
    </div>
  </div>
</template>
<script>
import VideoPlayer from "nuxt-video-player";
require("nuxt-video-player/src/assets/css/main.css");

export default {
  components: {
    VideoPlayer
  },
  async asyncData({ params }) {
    console.log("params", parseInt(params.idCurso) - 1);

    const dataCourses = ["Google Classroom", "Google Meet", "Zoom"];
    let titleCourse = dataCourses[parseInt(params.idCurso) - 1];
    let titlesVideo = [];
    if (parseInt(params.idCurso) == 1) {
      titlesVideo = [
        {
          title: "Guía rápida primeros pasos",
          number: 1,
          url: "/cursos/1/1"
        },
        {
          title: "Crea temas, material y tareas",
          number: 2,
          url: "/cursos/1/2"
        },
        {
          title: "Asignar y calificar tareas",
          number: 3,
          url: "/cursos/1/3"
        },
        {
          title: "Crear rubricas",
          number: 4,
          url: "/cursos/1/4"
        }
      ];
    } else if (parseInt(params.idCurso) == 2) {
      titlesVideo = [
        {
          title: "En pc y en Celular",
          number: 1,
          url: "/cursos/2/1"
        },
        {
          title: "La pizarra virtual",
          number: 2,
          url: "/cursos/2/2"
        },
        {
          title: "Programar reuniones con google calendar",
          number: 3,
          url: "/cursos/2/3"
        },
      ];
    } else if (parseInt(params.idCurso) == 3) {
      titlesVideo = [
        {
          title: "Crear reunión, grabar y compartir",
          number: 1,
          url: "/cursos/3/1"
        },
        {
          title: "Crear salas pequeñas en una reunión",
          number: 2,
          url: "/cursos/3/2"
        },
        {
          title: "La pizarra y sus herramientas",
          number: 3,
          url: "/cursos/3/3"
        },
      ];
    }
    return {
      course: {
        title: titleCourse,
        number: params.idCurso
      },
      video: {
        title: titlesVideo[parseInt(params.idVideo) - 1].title,
        number: params.idVideo,
        views: 151,
        url: "https://andrescarrasco.com/videos/" + params.idCurso + "-" + params.idVideo + ".mp4"
      },
      videos: titlesVideo
    };
  }
};
</script>
<style>
.content-class {
  margin-top: 20px;
}
</style>
