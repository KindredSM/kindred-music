<template>
  <nav class="navbar">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
    <a class="github" target="_blank" href="https://github.com/KindredSM"
      >GitHub</a
    >

    <a class="Email" target="_blank" href="mailto:kdsm@protonmail.com"
      >Contact</a
    >
  </nav>
  <router-view />

  <footer>
    <a class="email" href="mailto:kdsm@protonmail.com"
      ><h3>kdsm@protonmail.com</h3></a
    >
  </footer>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;300&display=swap");

body {
  background-color: black;
  background-image: url("/src/assets/bg.jpg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
#app {
  font-family: "Poppins", sans-serif;
  text-align: center;
  color: #e6e5e5;
}

.navbar {
  display: flex;
  justify-content: flex-end;
  padding: 30px;
  gap: 20px;

  .logo {
    display: flex;
    width: 100px;
  }

  a {
    font-weight: bold;
    color: #ffffff;
    text-decoration: none;
    transition: ease 0.2s;

    &:hover {
      transition: ease 0.2s;
      color: #9d9d9d;
    }

    &.router-link-exact-active {
      color: #9d9d9d;
    }
  }
}
.video {
  position: fixed;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
}
.email {
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  text-decoration: none;
  transition: ease 0.2s;

  &:hover {
    transition: ease 0.2s;
    color: #9d9d9d;
  }
}

@media screen and (max-width: 960px) {
  .navbar {
    display: flex;
    justify-content: center;
  }
  body {
    padding-bottom: 10rem;
  }
}
</style>
