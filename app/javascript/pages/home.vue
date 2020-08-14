<template>
  <div id='app'>
    <div class="header">
      <p>{{ message }}</p>
    </div>
    <div class="body">
      <top/>
      <right/>
      <left/>
      <bottom/>
    </div>
  </div>
</template>

<script>
import Top from "../layouts/Top.vue";
import Right from "../layouts/Right.vue";
import Bottom from "../layouts/Bottom.vue";
import Left from "../layouts/Left.vue";

export default {
  components: {
    Top,
    Right,
    Bottom,
    Left
  },
  data: function () {
    return {
      message: "Where are we going?"
    }
  }
}
</script>

<style scoped>
  p {
    font-size: 2em;
    text-align: center;
  }
  .body {
    display: flex;
    justify-content: space-evenly;
  }
</style>
