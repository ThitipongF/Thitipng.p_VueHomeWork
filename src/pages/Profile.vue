<template>
  <body>
    <div class="container">
      <h1>Profile</h1>
      <br />
    </div>
    <p>ชื่อ : {{ Name }}</p>
    <p>ชื่อเล่น : {{ Nname }}</p>
    <p>อายุ : {{ Age }}</p>
    <p>วันเกิด : {{ BDay }}</p>
    <p>กรุ๊ปเลือด : {{ Blood }}</p>
    <p>น้ำหนัก : {{ Weight }}</p>
    <p>ส่วนสูง : {{ Height }}</p>
    <p>ทักษะ : {{ Skill }}</p>
    <h2>
      <div class="container">
        <div>
          <router-link :to="{ name: 'Main' }"
            ><button>Main</button></router-link
          >
          &nbsp;&nbsp;&nbsp;
          <router-link :to="{ name: 'Contact' }"
            ><button>Contact</button></router-link
          >
        </div>
      </div>
    </h2>
  </body>
</template>

<script>
export default {
  data: () => ({
    Name: "ฐิติพงศ์ ผลพอตน",
    Nname: "ฟลุ๊ค",
    Age: "22",
    BDay: "24 มีนาคม 2542",
    Blood: "O",
    Weight: "80",
    Height: "173",
    Skill: "C#,SQL,PL,HTML,PHP,R,Python,JAVA,Power BI,",
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
  background-color: lightblue;
}
button {
  margin: 20px 20px 20px 20px;
  width: 100px;
  height: 100px;
  font-size: 0.6cm;
  color: blue;
}
</style>