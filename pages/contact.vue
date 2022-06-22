<template>
  <div>
    <Header />
    <section class="contact">
      <h1 class="contact__headline">Let's talk</h1>
      <p class="contact__text">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio, est
        natus? Maxime inventore magni laboriosam libero vel beatae!
      </p>
    </section>
    <form action="" class="form">
      <input type="text" class="form__input" placeholder="Name" />
      <input type="email" class="form__input" placeholder="Email" />
      <textarea
        name="message"
        id="message"
        cols="30"
        rows="10"
        class="form__input"
        placeholder="Message"
      ></textarea>
      <button type="submit" class="form__button">Send</button>
    </form>
  </div>
</template>

<style scoped>
.contact {
  display: flex;
  flex-direction: column;
  padding: 10pt 40pt 100pt 40pt;
}
.contact__headline {
  font-size: 7em;
  font-weight: 900;
}
.contact__text {
  max-width: 370pt;
  line-height: 1.7em;
}
.form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.form__input {
  width: 30em;
  padding: 4pt;
  margin: 7pt;
  background: #ffffff44;
  border: solid thin #ffffff55;
}
.form__button {
  padding: 4pt 7pt;
  margin: 10pt;
}
</style>
