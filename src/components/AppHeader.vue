<script>

export default {
  name: "AppHeader",
  props: {
    links: Object
  },
  data() {
    return {
    }
  }
}
</script>

<template>
  <div class="container">
    <div class="row align-items-center">
      <div class="col-2 py-2">
        <img src="/public/dc-logo.png" alt="" class="logo">
      </div>
      <div class="col-10">
        <ul class="nav justify-content-end">
          <li class="nav-item" v-for="(link, c) in links">
            <a class="nav-link active text-dark" aria-current="page" href="" v-if="link.status == true">{{
              link.link.toUpperCase() }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.logo {
  width: 50px;
}

.nav-item a:hover {
  border-bottom: solid 3px;
}
</style>

