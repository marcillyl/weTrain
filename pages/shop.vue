<template>
  <div>
    <Header />
    <section class="shop">
      <h1 class="shop__headline">The shop</h1>
      <p class="shop__text">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio, est
        natus? Maxime inventore magni laboriosam libero vel beatae!
      </p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Illum, nostrum a
      ab, soluta iusto in minus eum voluptas quia nam facilis quaerat
      consequuntur, placeat dolores veritatis modi possimus nisi amet.
    </section>
    <section class="articles">
      <h4>Articles</h4>
      <Product
        status="order"
        v-for="product in products"
        :name="product.name"
        :price="product.price"
        :key="product.id"
        v-on:order="addProduct"
      />
    </section>
    <section class="articles">
      <h4>Ordered</h4>
      <Product
        status="ordered"
        v-for="product in order"
        :name="product.name"
        :price="product.price"
        :key="product.id"
      />
    </section>
  </div>
</template>

<script>
import Product from "@/components/Product.vue";
export default {
  components: {
    Product,
  },
  data() {
    return {
      products: [
        { id: 1, name: "amet", price: 14.0 },
        { id: 2, name: "adipisicing", price: 1.0 },
        { id: 3, name: "dolor", price: 4.0 },
        { id: 4, name: "ipsum", price: 7.0 },
      ],
      order: [],
    };
  },
  methods: {
    addProduct(name, price) {
      console.log("ok");
      this.order.push({ name: name, price: price });
    },
  },
};
</script>

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
.articles {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
