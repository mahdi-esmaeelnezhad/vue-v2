<template>
  <div>
    <button @click="click">{{ add }}</button>
    <button @click="EverClickHandler">ever click</button>
    <button @click="changeEmitHandler">emit Change data</button>
  </div>
</template>

<script>
export default {
  name: "BtnCard",
  props:{
    EverClickHandler : Function
  },
  data() {
    return {
      add: "add",
    };
  },
  methods: {
    click: function () {
      this.add = "addddd";
    },
    changeEmitHandler(){
        this.$emit("changeEmitHandlerFunc" , "changed")
    }
  },
  mounted() {
    console.log("mahdi0");
  },
  beforeUpdate() {
    console.log("mahdi1");
  },
  updated() {
    console.log("mahdi2");
  },
};
</script>

<style></style>
