<template>
  <div class="home">
    <ProjectCard></ProjectCard>
  </div>
</template>

<script>
// @ is an alias to /src
import ProjectCard from '@/components/ProjectCard.vue'

export default {
  name: 'home',
  components: [ProjectCard]
}
</script>
