<template>
  <div class="card">
    <nav>
      <div class="title">
        <h2>All Customers</h2>
        <p>Active Members</p>
      </div>
      <form action="#">
        <input type="text" placeholder="Search..." />
        <select name="Short by : Newest" id="Short by : Newest">
          <option value="">Newest</option>
          <option value="">Oldest</option>
          <option value="">Alphabetically</option>
        </select>
      </form>
    </nav>
    <!-- table -->
    <Table />
    <footer>
      <p>Showing data 1 to 8 of 256K entries</p>
      <div class="flex">
        <button><i class="bi bi-chevron-left"></i></button>
        <button><i class="bi bi-1-square"></i></button>
        <button><i class="bi bi-2-square"></i></button>
        <button><i class="bi bi-3-square"></i></button>
        <button><i class="bi bi-chevron-right"></i></button>
      </div>
    </footer>
  </div>
</template>

<script setup>
import Table from '../table/index.vue'
</script>

<style lang="scss" scoped src="./_style.scss">
</style>
