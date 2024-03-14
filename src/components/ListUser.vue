<template>
  <div>
    <ul>
      <!-- <li>{{ item.name }}</li>
      <li>{{ item.age }}</li>
      <button @click="delete(item.id)">remove</button> -->
      <li v-for="item in users" :key="item.id">
        <p>{{ item.name }}</p>
        <button v-color="item.color" @click="deleteUser(item.id)">
          remove
        </button>
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
    deleteUser(id) {
      this.$emit("deleteItem", id);
    },
  },
  directives: {
    color: {
      bind(el, binding) {
        el.style.backgroundColor = binding.value;
      },
    },
  },
};
</script>

<style></style>
