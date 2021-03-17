<template>
  <div class="resume-content card col-md-8">
    <ResumeContentCard
      :title="cardDetails.languages.title"
      :list="cardDetails.languages.list"
      :links="cardDetails.languages.links"
    />
    <ResumeContentCard
      :title="cardDetails.skills.title"
      :list="cardDetails.skills.list"
      :links="cardDetails.skills.links"
    />
    <ResumeContentCard
      :title="cardDetails.tools.title"
      :list="cardDetails.tools.list"
      :links="cardDetails.tools.links"
    />
    <ResumeContentCard
      :title="cardDetails.certifications.title"
      :list="cardDetails.certifications.list"
      :links="cardDetails.certifications.links"
    />
  </div>
</template>

<style scoped>
.resume-content {
  padding: 20px;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(3, max-content);
  grid-row-gap: 20px;
}
</style>

<script>
import ResumeContentCard from "./ResumeContentCard.vue";

export default {
  name: "ResumeContent",
  components: {
    ResumeContentCard
  },
  data: function() {
    return {
      cardDetails: {
        languages: {
          title: "Languages 🦜",
          list: [
            "TypeScript",
            "Node.js/JavaScript",
            "Python (occasional)",
            "Go (occasional)",
            "SQL"
          ],
          links: []
        },
        skills: {
          title: "Skills 🌱",
          list: [
            "API Design",
            "Frontend Development",
            "CI",
            "Unit/Integration Testing",
            "Serverless Computing"
          ],
          links: []
        },
        tools: {
          title: "Tools 🦕",
          list: [
            "AWS, GCP",
            "Terraform",
            "Docker",
            "Ember.js, Vue.js, React (occasional)",
            "MySQL, MariaDB, PostgreSQL",
            "Redis"
          ],
          links: []
        },
        certifications: {
          title: "Certifications 🏆",
          list: [],
          links: [
            {
              url:
                "https://www.youracclaim.com/badges/5b5bc9f1-7cdf-4a00-b9f0-3cf22ac50848/public_url",
              text: "AWS Certified Solutions Architect – Associate (February 2020)"
            }
          ]
        }
      }
    };
  }
};
</script>

<style scoped>
@media (max-width: 800px) {
  .skill-header {
    text-align: center;
  }
}
</style>
