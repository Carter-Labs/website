<template>
 <form class="card email" accept-charset="utf-8" :action="EmailAction" method="POST">
  <h1>Contact Us</h1>
  <div class="form-group">
    <label for="name">Name</label>
    <input type="text" name="name" placeholder="Name" v-model="Name" required>
  </div>
  <div class="form-group">
    <label for="email">Email</label>
    <input type="email" name="email" placeholder="Email" v-model="Email" required>
  </div>
  <div class="form-group">
    <label for="message">Message</label>
    <textarea type="textarea" name="message" rows="6" placeholder="Message" v-model="Message" required></textarea>
  </div>
  <div class="form-group">
    <input type="submit" class="btn">
  </div>
  </form>
</template>

<script>
export default {
  data () {
    return {
      Name: '',
      Email: '',
      Message: ''
    }
  },
  computed: {
    EmailAction: () => {
      return 'https://formspree.io/contact@carterlabs.dev'
    }
  }
}
</script>
<style lang="sass" scoped>
.email
  text-align: left
  h1
    margin: 0
    font-size: 150%
  .form-group input, textarea
    width: 100%
    border: 1px solid #536dfe;
    border-radius: 2px;
    clear: both
    text-indent: 1%
    padding: 1% 0
    textarea
      resize: vertical
</style>
