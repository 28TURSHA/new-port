<template>
  <h1 class="headin d-flex justify-content-center">
    <span style="color: #1e90ff">Projects</span>
  </h1>
  <div class="project-container">
    <div class="project-card" v-for="project in projects" :key="project.id">
      <img class="image" :src="project.img" alt="" />
      <div class="project-overlay">
        <h4>{{ project.title }}</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [],
      //   loading: false,
    };
  },
  //   components: { Loader },
  mounted() {
    this.loading = true;
    fetch("https://backend-tursha.herokuapp.com/projects")
      .then((res) => res.json())
      .then((data) => {
        this.projects = data;
        this.loading = false;
      })
      .catch((err) => console.log(err.message));
  },
};
</script>
<style scoped>
h1 {
  padding-top: 150px;
}

p {
  position: relative;
  bottom: 55px;
  color: white;
}
.project-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 3rem;
  margin: 2rem 0;
  padding: 0;
  width: 100%;
}
.project-card {
  background: #1f1f1f;
  max-width: 30%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  position: relative;
}
.image {
  display: block;
  width: 400px;
  width: 100%;
  height: auto;
  object-fit: cover;
}
.project-overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: 0.5s all;
  background-color: rgba(0, 0, 0, 80%);
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}
.project-card:hover .project-overlay {
  opacity: 1;
}
</style>
