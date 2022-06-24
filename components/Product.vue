<template>
  <div>
    <article class="article">
      <h3 class="article__headline">{{ name }}</h3>
      <p class="article__text">Price : {{ price }} $</p>
      <button v-if="status == 'order'" @click="$emit('order', name, price)" class="article__button">Buy</button>
    </article>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: ["name", "price", "status"],
};
</script>


<style scoped>
.article {
  width: 100pt;
  height: 100pt;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: #ffffff44;
  border: solid thin #ffffff55;
  margin: 10pt;
  padding: 10pt;
}
.article__headline {
  font-size: 1.4em;
  font-weight: 700;
}
.article__text {
  margin: 10pt 0;
}
</style>
