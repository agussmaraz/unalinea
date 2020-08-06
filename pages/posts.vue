<template>
  <div>

    <nuxt-child />
  </div>
</template>

<script>
export default {
  data() {
    return {
      postId: ""
    };
  },
  methods: {
    onLoadPost() {
      this.$router.push("/posts/" + this.postId);
      return true;
    }
  }
};
</script>

<style></style>
