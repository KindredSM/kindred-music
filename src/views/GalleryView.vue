<template>
  <h1 class="header">Gallery</h1>
  <div class="gallery-grid">
    <img
      src="@/assets/cyberpunk.jpeg"
      class="gallery-image"
      alt="gallery image"
      srcset=""
    />
    <img
      src="@/assets/skull.jpeg"
      class="gallery-image"
      alt="gallery image"
      srcset=""
    />
    <img
      src="@/assets/redskull.jpeg"
      class="gallery-image"
      alt="gallery image"
      srcset=""
    />
    <img
      src="@/assets/woman.jpeg"
      class="gallery-image"
      alt="gallery image"
      srcset=""
    />
  </div>
</template>

<style lang="scss">
.gallery-grid {
  padding: 100px 0px 100px 0px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 1rem;
}
.gallery-image {
  width: 400px;
  border-radius: 3px;
}

@media screen and (max-width: 960px) {
  .gallery-grid {
    transform: scale(0.8);
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 8rem;
    padding: 0;
  }
}
</style>
