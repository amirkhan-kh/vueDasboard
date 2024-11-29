<template>
  <div class="wrapper">
    <Aside />
    <main>
      <Header />
      <section id="routing">
        <router-view></router-view>
      </section>
      <!-- <Footer /> -->
    </main>
  </div>
</template>

<script setup>
import Aside from '../../components/navigation/index.vue'
import Header from '../../components/header/index.vue'
// import Footer from '../../components/footer/index.vue'
</script>

<style lang="scss" scoped src="./_style.scss">
</style>
