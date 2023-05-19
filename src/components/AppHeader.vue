<script>

export default {
  name: "AppHeader",
  data() {
    return {
      links: [
        {
          link: 'Characters',
          status: true
        },
        {
          link: 'Comics',
          status: true
        },
        {
          link: 'Movies',
          status: true
        },
        {
          link: 'TV',
          status: true
        },
        {
          link: 'Games',
          status: true
        },
        {
          link: 'Collectibles',
          status: true
        },
        {
          link: 'Videos',
          status: true
        },
        {
          link: 'Fans',
          status: true
        },
        {
          link: 'News',
          status: true
        },
        {
          link: 'Shop',
          status: true
        },
      ]
    }
  }
}
</script>

<template>
  <div class="container">
    <div class="row  py-2 align-items-center">
      <div class="col-2">
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
</style>

