<template>
  <body>
    <h1>
      <div class="container">
        <div>
          <router-link :to="{ name: 'Profile' }"
            ><button>Profile</button></router-link
          >
          &nbsp;&nbsp;&nbsp;
          <router-link :to="{ name: 'Contact' }"
            ><button>Contact</button></router-link
          >
        </div>
      </div>
    </h1>
  </body>
</template>

<style scoped>
h1 {
  font-size: 3em;
  text-align: center;
}
body {
  margin: 250px 50px 250px 50px;
}
button {
  margin: 20px 20px 20px 20px;
  width: 100px;
  height: 100px;
  font-size: 0.6cm;
  color: blue;
}
</style>