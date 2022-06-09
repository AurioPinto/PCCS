<template>
<div class="logtop">
  <div class="sides">
    <div class="right">
      <img src="./assets/hbs.png" alt="">
    </div>
    <div class="left">
      <img src="./assets/PCComputerServiceLogo.png" alt="">
    </div>
  </div>
</div>
  <!-- <header>
    <div class="app">
      <div id="nav"></div>
      <div class="layers">
        <div class="profile">
          <div class="img">
            <router-link to="/">
              <img src="./assets/PCComputerServiceLogo.png" alt />
            </router-link>
          </div>
          <div class="profile-name">
            <h2>{{ profilename }}</h2>
          </div>
        </div>
        <div class="navigation">
          <router-link to="/"> <span>Home</span> </router-link>|
          <router-link to="/"> <span>Handel</span> </router-link>|
          <router-link to="/"> <span>Beratung</span> </router-link>
        </div>
      </div>
      <router-view />
    </div>
  </header> -->
</template>

<script>
// import project from "./components/projects.vue";

export default {
  name: "app",
  data() {
    return {
      user: {
        name: "app"
      },
      profilename: "PC COMPUTER SERVICES"
    };
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Spirax&display=swap");
$primary-color: #17a2b8;
$dark-color: #343a40;
$back-color: #333;
$light-color: #f4f4f4;
$danger-color: #dc3545;
$west-color: #ffff;
$success-color: #28a745;

.logtop{
  .sides{
    display: flex;
    justify-content: space-around;
    padding-top: 20px;
    // .right{}
  }
}

.profile {
  text-align: center;
  margin-bottom: 10px;
  color: $back-color;
  h2 {
    line-height: 1.5;
    font-family: "Spirax", cursive;
    color: #004b64;
  }
}
.profile-name {
  font-size: 20px;
  margin-top: 10px;
  color: $back-color;
}
.img img {
  width: 150px;
  border-radius: 88px;
  margin-top: 10px;
}
.layers {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1030;
  background-color: #99CCFF;
}
.navigation {
  text-align: center;
  font-size: 1.4rem;
  margin-top: 20px;
  span {
    margin: 0 25px;
    cursor: pointer;
    color: #333;
    text-decoration: none;
  }
  a {
    text-decoration: none;
  }

  span:hover {
    border-bottom: 5px solid #00263c;
    color: #f8991d;
  }
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000;
}
body {
  margin: 0;
  font-family: "Lato" sans-serif;
}
body::-webkit-scrollbar {
  display: none !important;
}
* {
  margin: 0;
  padding: 0;
  margin-block-start: 0;
  margin-block-end: 0;
  margin-inline-start: 0;
  margin-inline-end: 0;
}
html,
body {
  height: 100%;
  background-color: #99CCFF;
}
</style>
