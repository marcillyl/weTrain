<template>
  <div>
    <Header />
    <section class="shop">
      <h1 class="shop__headline">The shop</h1>
      <p class="shop__text">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio, est
        natus? Maxime inventore magni laboriosam libero vel beatae!
      </p>
    </section>
  </div>
</template>

<style>
.shop {
  display: flex;
  flex-direction: column;
  padding: 10pt 40pt 100pt 40pt;
}
.shop__headline {
  font-size: 7em;
  font-weight: 900;
}
.shop__text {
  max-width: 370pt;
  line-height: 1.7em;
}
</style>
