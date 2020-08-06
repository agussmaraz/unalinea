<template>
  <div class="home-page">
    <section class="title-posts">
      <h1>Get the lastest tech news!</h1>
    </section>
    <section class="featured-posts">
      <postPreview
        id="1"
        thumbnail="https://miro.medium.com/max/3004/0*ayP9NP9sD9xxB5PI"
        title="Post 1"
        previewText="hola"
      />
      <postPreview
        id="2"
        thumbnail="https://miro.medium.com/max/3004/0*ayP9NP9sD9xxB5PI"
        title="Post 2"
        previewText="hola"
      />
      <postPreview
        id="3"
        thumbnail="https://miro.medium.com/max/3004/0*ayP9NP9sD9xxB5PI"
        title="Post 3"
        previewText="hola"
      />
    </section>
  </div>
</template>

<script>
import postPreview from "~/components/Posts/postPreview";
export default {
  components: {
    postPreview
  }
};
</script>
<style scoped>
.title-posts {
  text-align: center;
  font-size: 40px;
}
.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
