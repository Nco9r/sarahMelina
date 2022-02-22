<template>
  <section class="projets">
    <div class="items_projets">
      <div class="item">
        <div class="title_item">
          <h3>Ensemble, donnons vie à vos idées avec créativité.</h3>
        </div>
        <div class="realisation">
          <div class="cta_rea">
            <p>Voir mes réalisations</p>
            <img src="~assets/img/svg/next.svg" alt="" />
          </div>
          <hr />
        </div>
      </div>
      <div class="img">
        <img src="~assets/img/jpg/projets_1.jpg" alt="" />
      </div>
      <div class="img">
        <img src="~assets/img/jpg/projets_2.jpg" alt="" />
      </div>
      <div class="img">
        <img src="~assets/img/jpg/projets_3.jpg" alt="" />
      </div>
      <div class="img">
        <img src="~assets/img/jpg/projets_5.jpg" alt="" />
      </div>
      <div class="img">
        <img src="~assets/img/jpg/projets_6.jpg" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.projets {
  background: rgb(255, 217, 223);
  background: -moz-linear-gradient(
    180deg,
    rgba(255, 217, 223, 1) 0%,
    rgba(255, 255, 255, 1) 100%
  );
  background: -webkit-linear-gradient(
    180deg,
    rgba(255, 217, 223, 1) 0%,
    rgba(255, 255, 255, 1) 100%
  );
  background: linear-gradient(
    180deg,
    rgba(255, 217, 223, 1) 0%,
    rgba(255, 255, 255, 1) 100%
  );
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#ffd9df",endColorstr="#ffffff",GradientType=1);
}

.items_projets {
  display: flex;
  flex-flow: column;
  padding: 15px 15px 15px 15px;
}

.item {
  width: 100%;
  height: 500px;
  background-color: var(--yellow);
  border-radius: 6px;
  position: relative;
  margin-bottom: 15px;
}

.img img {
  width: 100%;
  height: 500px;
  object-fit: cover;
  border-radius: 6px;
  position: relative;
  margin-bottom: 15px;
}

.title_item h3 {
  width: 200px;
  padding: 15px;
  line-height: 46px;
  font-size: 36px;
  font-weight: 900;
}

.realisation {
  position: absolute;
  bottom: 40px;
  left: 20px;
}

.cta_rea {
  display: flex;
  align-items: center;
}

.cta_rea p {
  font-size: 18px;
  font-weight: 900;
  margin-right: 20px;
}

.cta_rea img {
  width: 30px;
  margin-top: 5px;
}

hr {
  border: none;
  height: 2px;
  width: 100%;
  background-color: var(--black);
  margin-top: 20px;
}
</style>
