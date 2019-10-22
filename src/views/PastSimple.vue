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
  </div>
</template>

<script>
export default {
  name: "pastSimple",
  components: {}
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
