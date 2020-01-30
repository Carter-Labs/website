<template>
  <nav>
    <div class="branding"></div>
    <div class="tabs">
      <router-link class="tab" to="/">Home</router-link>
      <router-link class="tab" to="/about">About</router-link>
    </div>
  </nav>
</template>
<style lang="sass" scoped>
nav
  display: grid
  grid-template-columns: 1fr 3fr
  padding: 1.5% 3%
  margin-bottom: 4%
  background-color: #448aff
  box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
.tabs
  text-align: right
.tab
  color: #ffffff
  text-decoration: none
  padding: .5% 4%
  font-size: 1.25em
  &:hover
    background-color: rgba(83,109,254,0.5)
.tab.router-link-exact-active
  border-bottom: 2px solid #ffffff
</style>
