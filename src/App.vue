<template>
  <router-view></router-view>
</template>

<script>
// import CardShow from "./components/ShowCard";
// import BtnCard from "./components/Button";
// import ListUser from "./components/ListUser";

// export default {
//   name: "App",
//   components: {
//     CardShow,
//     BtnCard,
//     ListUser,
//   },
//   data() {
//     return {
//       clickApp: "click app",
//       user: [
//         { name: "mahdi", age: 22, id: 1, color : "red" },
//         { name: "sara", age: 24, id: 2, color : "green" },
//       ],
//     };
//   },
//   methods: {
//     removeUser(id) {
//      let userItem = this.user.findIndex((item) => item.id == id);
//       // console.log(user);
//       this.user.splice(userItem , 1)
//       console.log(userItem)
//     },
//     clickAppHandler: function () {
//       this.clickApp = "app";
//     },
//     clickHandlers: function () {
//       alert("mahdi");
//     },
//     changeEmit: function (data) {
//       console.log(data);
//     },
//   },
//   beforeUpdate() {
//     console.log("mahdiapp");
//   },
//   updated() {
//     console.log("mahdiapp2");
//   },
// };
</script>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
