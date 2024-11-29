<template>
  <div class="table">
    <table>
      <thead>
        <tr class="tr">
          <th>Customer Name</th>
          <th>Company</th>
          <th>Phone Number</th>
          <th>Email</th>
          <th>Country</th>
          <th style="padding-left: 70px">Status</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="el in tableData" :key="el">
          <td>{{ el.name }}</td>
          <td>{{ el.compony }}</td>
          <td>{{ el.phone }}</td>
          <td>{{ el.email }}</td>
          <td>{{ el.country }}</td>
          <td>
            <button
              :class="{
                'active-button': user.status === 'Active',
                'inactive-button': user.status === 'Inactive',
              }"
            >
              {{ user.status }}
            </button>
          </td>
          <td></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import { tableData } from '../../../constants/index.js'
const user = {
  status: 'Active',
}
</script>

<style lang="scss" scoped src="./_style.scss">
</style>
