<template>
  <div id="app">
    <div id="app-container" class="container mx-auto d-flex flex-column justify-content-between">
      <div class="page-header d-flex justify-content-between">
        <div class="left">
          <h1>Kaley Kriminger</h1>
          <h2 id="job-title" class="text-muted lh-1">
            Software Engineer
          </h2>
        </div>
        <div class="right align-self-center">
          <a class="mail-button button btn btn-default btn-lg" href="mailto:kaley.kriminger@gmail.com">Contact me</a>
        </div>
      </div>
      <div class="main-content d-flex justify-content-around mb-4">
        <div class="about-me align-self-center">
          <h5>Hello!</h5>
          <p>I'm a Software Engineer with over 7 years of experience building well-tested, reliable systems in the cloud.</p>
          <p>My primary tools are Go, Python, and TypeScript/Node.js, and I also have experience building user interfaces with JavaScript, React, and HTML/CSS.</p>
          <p>If you'd like to connect, feel free to drop me an <a href="mailto:kaley.kriminger@gmail.com">email</a>.</p>
        </div>
        <div class="">
          <div class="card text-center" style="width: 24rem;">
            <img class="card-img-top" src="./assets/kaley.jpeg" alt="kaley" />
          </div>
        </div>
      </div>
      <div class="d-flex flex-row justify-content-center">
          <a href="https://www.linkedin.com/in/kaleykriminger/"><img src="./assets/linkedin.png" alt="linkedin logo" /></a>
          <a href="https://github.com/KaleyKrim"><img src="./assets/github.png" alt="github logo" /></a>
      </div>
      </div>
  </div>
</template>

<script>
export default {
  name: "app",
};
</script>

<style>
.main-content {
  display: flex;
  flex-direction: column-reverse;
}
.page-header {
  display: flex;
  flex-direction: column;
  margin-bottom: 15px;
}
.about-me {
  margin-top: 15px;
}
#job-title {
margin-top: -15px;
}
.page-header {
width: 100%;
}
#button-primary {
  color: #E2EAEC;
}
#button-secondary {
  color: #CBD8A6
}
#app {
background-color: #A7D8D5;
height: 100vh;
}
#app-container {
background-color: white;
height: 100%;
padding: 35px;
}
.mail-button {
color: white !important;
background-color: black !important;
}
.mail-button:hover {
background-color: #3d3d3d !important;
}
.about-me {
  max-width: 500px;
}
@media only screen and (min-width: 480px) {
  .page-header {
   display: flex;
   flex-direction: row;
   margin-bottom: 0;
  }
}
@media only screen and (min-width: 768px) {
  .main-content {
    display: flex;
    flex-direction: row;
  }
  .about-me {
    margin-top: 0;
  }
}
</style>
