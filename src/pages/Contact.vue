<template>
  <body>
    <div class="container">
      <h1>Contact</h1>
      <br />
    </div>
    <p>เบอร์โทร :{{ Phone }}</p>
    <p>Email :{{ Email }}</p>
    <h2>
      <div class="container">
        <div>
          <router-link :to="{ name: 'Main' }"
            ><button>Main</button></router-link
          >
          &nbsp;&nbsp;&nbsp;
          <router-link :to="{ name: 'Profile' }"
            ><button>Profile</button></router-link
          >
        </div>
      </div>
    </h2>
  </body>
</template>

<script>
export default {
  data: () => ({
    Phone: "062-5641582",
    Email: "Thitipong2442@gmail.com",
  }),
};
</script>

<style scoped>
h1,
h2 {
  font-size: 3em;
  text-align: center;
}
p {
  font-size: 1em;
  margin: 20px 0px 0px 20px;
}
body {
  background-color: lightgreen;
}
button {
  margin: 20px 20px 20px 20px;
  width: 100px;
  height: 100px;
  font-size: 0.6cm;
  color: blue;
}
</style>