<template>
  <div id="app" class="container">
    <div class="text-center page-header">
      <h1 class="display-2">Kaley Kriminger</h1>
      <h3 id="job-title">
        Software Developer
        <small class="text-muted">
          { Backend ・ DevOps ・ Full Stack }
        </small>
      </h3>
    </div>
    <br />
    <div class="row justify-content-center">
      <div class="col-4">
        <div class="card text-center bg-dark text-white" style="width: 18rem;">
          <h5 class="card-header">Contact me!</h5>
          <img class="card-img-top" src="./assets/kaley.png" alt="kaley" />
          <div class="card-body">
            <p class="card-text">I'm currently looking for a back end or full stack position. (Within the US or remote)</p>
            <ul class="list-group">
              <li class="list-group-item">
                <a href="mailto:kaley.kriminger@gmail.com">✉️ Email</a>
              </li>
              <li class="list-group-item">
                <a href="https://github.com/KaleyKrim">🐙 Github</a>
              </li>
              <li class="list-group-item">
                <a href="https://www.linkedin.com/in/kaleykriminger/">🔗 LinkedIn</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-6">
        <ResumeContent />
      </div>
    </div>
  </div>
</template>

<script>
import ResumeContent from "./components/ResumeContent.vue";

export default {
  name: "app",
  components: {
    ResumeContent
  }
};
</script>

<style>
/* #my-face {
  max-width: 250px;
} */
#job-title {
  color: #00d5a4;
}
</style>
