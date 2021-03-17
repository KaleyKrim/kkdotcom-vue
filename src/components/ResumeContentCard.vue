<template>
  <div class="row resume-content-card">
    <div class="col-12 skill-header">
      <h3>{{ title }}</h3>
    </div>
    <div class="row">
      <div class="col">
        <ul v-if="links">
          <li v-for="(item, index) in list" :key="index">
            {{ item }}
          </li>
          <li v-for="(item, index) in links" :key="index">
            <a :href="item.url">{{ item.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>

<script>
export default {
  name: "ResumeContentCard",
  props: {
    title: {
      type: String
    },
    list: {
      type: Array
    },
    links: {
      type: Array
    }
  }
};
</script>

<style>
#job-title {
  color: #00d5a4;
}
</style>
