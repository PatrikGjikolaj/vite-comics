<script>

export default {
  name: "AppHeader",
  data() {
    return {
      links: [
        {
          link: 'Characters',
        },
        {
          link: 'Comics',
        },
        {
          link: 'Movies',
        },
        {
          link: 'TV',
        },
        {
          link: 'Games',
        },
        {
          link: 'Collectibles',
        },
        {
          link: 'Videos',
        },
        {
          link: 'Fans',
        },
        {
          link: 'News',
        },
        {
          link: 'Shop',
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
            <a class="nav-link active text-dark" aria-current="page" href="">{{ link.link.toUpperCase() }}</a>
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

