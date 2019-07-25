<template>
  <div id="app">
    <div class="page">
      <div class="content">
        <div class="header">
          <div class="logo">Peopleawesome</div>
          <div class="btn" @click="open()"><i class="fal fa-bars"></i></div>
        </div>
        <div class="container">
          <div class="image">
            <img src="https://static.dezeen.com/uploads/2019/07/elon-musk-neuralink-technology_dezeen_2364_hero-1.jpg" alt="">
          </div>
          <h1>Elon Musk's Neuralink implant will "merge" humans with AI</h1>
          <div class="rating">
            <i class="fas fa-star selected"></i>
            <i class="fas fa-star selected"></i>
            <i class="fas fa-star selected"></i>
            <i class="fas fa-star selected"></i>
            <i class="fas fa-star"></i>
          </div>
          <p>The approaching technology would see groups of minuscule, flexible electrode "threads" implanted into the human brain by a neurosurgical robot.</p>
          <p>These threads detect and record the electrical signals in the brain, and transmit this information outside the body.</p>
        </div>
      </div>
      <div class="menu" :class="{ active: showMenu }">
        <div class="head">
          <div class="logo">Peopleawesome</div>
          <div class="btn" @click="close()"><i class="fal fa-times"></i></div>
        </div>
        <div class="item">Home</div>
        <div class="item">Article</div>
        <div class="item">Category</div>
        <div class="item">About</div>
      </div>
    </div>
  </div>
</template>

<script>
import '@fortawesome/fontawesome-pro/css/all.css'
export default {
  data () {
    return {
      showMenu: false
    }
  },
  methods: {
    open: function () {
      this.showMenu = true
    },
    close: function () {
      this.showMenu = false
    }
  }
}
</script>

<style lang="less">
@import '~@/assets/less/style';
</style>
