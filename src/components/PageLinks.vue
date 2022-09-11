<template>
  <div class="links-container">
    <h1 class="links">{{ msg }}</h1>
  </div>
</template>

<style lang="scss">
.links {
  color: rgb(255, 255, 255);
  font-size: 2rem;
  font-weight: 100;
  display: flex;
  align-items: center;
  text-align: justify;
  text-decoration: none;
  justify-content: center;
  padding: 10px;
  width: fit-content;
  margin: 0 auto;
  transition: all ease 0.2s;

  &:hover {
    transition: all ease 0.2s;
    color: black;
    transform: scale(1.02);
    background-color: rgb(255, 255, 255);
  }
}
</style>

<script>
export default {
  name: "PageLinks",
  props: {
    msg: String,
  },
};
</script>
