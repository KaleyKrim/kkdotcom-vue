<template>
  <div id="app" class="container justify-content-center">
    <div class="text-center page-header">
      <h1 class="display-2">Kaley Kriminger</h1>
      <h3 id="job-title">
        Software Developer
      </h3>
      <small class="text-muted">
        Full Stack ・ Backend ・ DevOps
      </small>
    </div>
    <br />
    <div class="row justify-content-center ml-3">
      <div class="col-md-4 mb-4">
        <div class="card text-center bg-dark text-white" style="width: 18rem;">
          <h5 class="card-header">Contact me!</h5>
          <img class="card-img-top" src="./assets/kaley.jpeg" alt="kaley" />
          <div class="card-body">
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
      <ResumeContent />
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
#job-title {
  color: #00d5a4;
}
</style>
