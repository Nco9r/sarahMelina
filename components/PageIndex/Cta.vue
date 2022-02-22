<template>
  <section class="cta">
    <p>
      Une idée, un projet ? <br />
      Parlons en !
    </p>
    <div class="btn">
      <button>Devis gratuit</button>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.cta {
  height: 400px;
  background-image: url('~assets/img/jpg/cta.jpg');
  background-size: cover;
  background-position: 30% 50%;
  text-align: center;
}

.cta p {
  padding: 70px 0 30px 0;
  text-align: center;
  font-size: 36px;
  color: var(--white);
  font-weight: 900;
}

.btn button {
  text-align: center;
  margin: 20px auto;
  background-color: var(--yellow);
  color: var(--black);
  font-weight: 900;
}
</style>
