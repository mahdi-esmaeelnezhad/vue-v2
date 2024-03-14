<template>
  <div>
    <ul>
      <!-- <li>{{ item.name }}</li>
      <li>{{ item.age }}</li>
      <button @click="delete(item.id)">remove</button> -->
      <li  v-for="item in users" :key="item.id">
        <p>{{ item.name }}</p>
        <button @click="deleteUser(item.id)">remove</button>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  props: {
    users: Array,
  },
  methods: {    
    deleteUser(id){
      this.emit("deleteItem" , id)
        }
  }
};
</script>

<style></style>
