<template>
  <div class="home">
    <EmailCard></EmailCard>
  </div>
</template>

<script>
// @ is an alias to /src
import EmailCard from '@/components/EmailCard'

export default {
  name: 'home',
  components: {
    EmailCard
  }
}
</script>
