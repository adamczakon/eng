<template>
  <div class="container">
    <h1 class="text-secondary">Past Simple</h1>
    <p>Czasu Past Simple używamy do opisywania wydarzeń z przeszłości.</p>
    <h3>Szyk zdania twierdzącego prezetuje się następująco:</h3>
    <div class="align-center">
      <span class="introduction-border">
        Podmiot +
        <span class="text-primary">
          <strong>II forma czasownika</strong>
        </span> + reszta zdania
      </span>
    </div>
    <div class="excersise">
      He
      <input
        v-model="userAnswer"
        name="userAnswer"
        v-on:blur="handleAnswerCheck"
        class="input-excersise"
      /> (play) volleyball yesterday.
    </div>
  </div>
</template>

<script>
export default {
  name: "pastSimple",
  components: {},
  data() {
    return {
      correctAnswer: "played",
      userAnswer: ""
    };
  },
  methods: {
    handleAnswerCheck() {
      /* eslint-disable */
      console.log(this);
      this.correctAnswer === this.userAnswer && console.log("great");
    }
  }
};
</script>

<style scoped lang="scss">
.introduction-border {
  border: 1px solid $primary;
  border-radius: 20px;
  padding: 1rem 2rem;
  margin: 0 auto;
}

.align-center {
  display: flex;
  justify-content: center;
}

.input-excersise {
}
</style>
