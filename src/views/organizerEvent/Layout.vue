<template>
  <div v-if="GStore.event">
    <h1>ID: {{ GStore.event.id }}</h1>
    <div id="nav">
      <router-link :to="{ name: 'OrganizerDetail' }">Details</router-link>
      |
      <router-link :to="{ name: 'OrganizerRegister' }">Register</router-link>
      |
      <router-link :to="{ name: 'OrganizerEdit' }">Edit</router-link>
    </div>
    <router-view :event="GStore.event" />
  </div>
</template>
<script>
export default {
  inject: ['GStore']
}
</script>
