<template>
  <div id="shopping-list">
    <h1>{{ header || 'Welcome' }}</h1>

    <ul>
      <li v-for="item in items" :key="item.id">{{ item.label }}</li>
    </ul>
  </div>
</template>

<script>

export default {
  data() {
    return {
      header: 'Shopping List App',
      items: [
        { id: 1, label: "10 party hats" },
        { id: 2, label: "2 board games" },
        { id: 3, label: "20 cups" },
      ]
    }
  }
}

</script>

<style></style>
