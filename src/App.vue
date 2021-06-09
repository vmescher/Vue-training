<template>
  <div class="block">
    <form action="#" method="get" class="block__form form">
      <input
        class="form__input"
        v-model="message"
        type="text"
        placeholder="Введите текст"
      />
      <input
        type="submit"
        class="form__button"
        value="Подтвердить"
        @click="getName()"
      />
    </form>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      message: null,
    };
  },
  methods: {
    getName() {
      console.log(this.message);
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.block {
  max-width: 350px;
  margin: 0 auto;
}
</style>
