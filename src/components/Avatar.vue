<template>
  <div class="avatar">
    <img :src="imagen" alt="">
    <p>{{ nombre }}</p>
  </div>
</template>

<script>
export default {
  props: ["nombre", "imagen"]
}
</script>

<style>

.avatar {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin: 1rem;
}

img {
  border-radius: 50%;
  height: 72px;
  width: 72px;
}

p {
  color: rgb(222, 233, 222);
  margin: 0;
  font-size: 2rem;
}
</style>