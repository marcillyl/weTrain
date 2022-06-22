<template>
  <div>
    <main class="main">
      <h3 class="main__headline">What we do</h3>
      <div class="services">
        <article
          v-for="service in services"
          v-bind:key="service.id"
          class="card"
        >
          <h4 class="card__headline">{{ service.title }}</h4>
          <p class="card__text">{{ service.description }}</p>
        </article>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      services: [
        {
          id: 1,
          title: "Possimus",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores, quas! Esse a dignissimos illo distinctio excepturi repellat, fugiat odio.",
        },
        {
          id: 2,
          title: "In quae",
          description:
            "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Officia rem optio saepe asperiores obcaecati. , id numquam cum commodi.",
        },
        {
          id: 3,
          title: "Non, ratione",
          description:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fuga rerum rem repellendus quisquam unde quae accusamus perferendis corrupti deserunt!",
        },
      ],
    };
  },
};
</script>

<style>
.main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.main__headline {
  font-size: 3em;
  font-weight: 700;
  padding-bottom: 4pt;
  border-bottom: solid thick white;
  border-top: solid thick white;
}
.services {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 40pt 0;
}
.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: 170pt;
  background-color: #ffffff44;
  border: solid thin #ffffff55;
  margin: 10pt;
  padding: 10pt;
}
.card__headline {
  font-size: 1.7em;
  font-weight: 900;
  margin-bottom: 14pt;
}
</style>
