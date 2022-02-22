<template>
  <section class="insta">
    <img class="turn" src="~assets/img/svg/turn.svg" alt="" />
    <img class="insta_i" src="~assets/img/svg/insta_i.svg" alt="" />
    <div class="box_insta">
      <div class="title_insta">
        <h3>Retrouvez moi sur Instagram</h3>
      </div>
      <div class="avatar">
          <img src="~assets/img/jpg/avatar.png" alt="">
          <p>@by_sarahmelina</p>
      </div>
      <div class="trait">
          <img src="~assets/img/svg/trait.svg" alt="">
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
.insta {
  padding-bottom: 50px;
  background-color: var(--rose-secondary);
  position: relative;
}

.green {
    color: var(--green);
}

.turn {
  z-index: 0;
  margin-top: -50px;
  width: 100px;
  margin-left: 40px;
  animation: rotate 5s infinite linear;
}

@keyframes rotate {
    0% {
        transform: rotate(0);
    }
    100% {
        transform: rotate(360deg);
    }
}

.insta_i {
    position: absolute;
    right: 0;
}

.title_insta {
  text-align: center;
  padding: 0px 15px;
  z-index: 1;
}

.title_insta h3 {
  font-size: 32px;
  color: var(--white);
  font-weight: 900;
  z-index: 10;
  margin-top: 20px;
}

.avatar {
    text-align: center;
    margin-top: 30px;
}

.avatar img {
    width: 110px;
}


.avatar p{
    font-weight: 900;
    margin-top: 20px;
}

.trait {
    text-align: center;
    margin-top: 5px;
}
</style>
