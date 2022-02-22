<template>
  <section class="baseline">
    <div class="baseline_first">
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p class="stroke">Foodpreneur</p>
    </div>
    <div class="baseline_second">
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">pPreneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
      <p>Food<span class="gray">preneur</span></p>
      <img src="~assets/img/svg/star.svg" alt="" />
    </div>
  </section>
</template>

<script>
import { gsap } from 'gsap'
import { ScrollTrigger } from 'gsap/dist/ScrollTrigger'
gsap.registerPlugin(ScrollTrigger)

export default {
  mounted() {
    gsap.to('.baseline_first', {
      scrollTrigger: {
        trigger: '.baseline_first',
        start: '-10% 110%',
        end: 'top',
        scrub: true,
        toggleActions: 'restart pause reverse pause',
      },
      x: 900,
    }),
      gsap.to('.baseline_second', {
        scrollTrigger: {
          trigger: '.baseline_second',
          start: '-10% 110%',
          end: 'top',
          scrub: true,
          toggleActions: 'restart pause reverse pause',
        },
        x: -900,
      })
  },
}
</script>

<style scoped>
.baseline {
  overflow: hidden;
  height: 170px;
  margin-top: 50px;
}

.baseline_first {
  display: flex;
  flex-flow: row nowrap;
  margin-left: -900px;
}

.baseline_first .stroke {
  color: transparent;
  -webkit-text-stroke: 1px var(--black);
  font-size: 60px;
  line-height: 60px;
  text-transform: uppercase;
  margin-left: 7px;
  margin-right: 7px;
  font-weight: 900;
}

.baseline_first img {
  margin: 0 10px;
  width: 30px;
}

.baseline_second {
  display: flex;
  flex-flow: row nowrap;
  margin-left: 200px;
}

.baseline_second p {
  color: var(--black);
  font-size: 60px;
  line-height: 60px;
  text-transform: uppercase;
  font-weight: 900;
  margin-left: 7px;
  margin-right: 7px;
}

.baseline_second img {
  margin: 0 10px;
  width: 30px;
}

.baseline_second p .gray {
    color: var(--gray)!important;
    margin-top: 100px;
}

@media screen and (min-width: 1024px) {
  .baseline {
    margin-top: 60px;
    margin-bottom: 110px;
  }

  .baseline_first {
    margin-left: -1300px;
  }

  .baseline_second {
    margin-left: -200px;
  }

  .baseline_first p {
    font-size: 80px;
    line-height: 80px;
  }

  .baseline_second p {
    font-size: 80px;
    line-height: 80px;
  }
}

@media screen and (min-width: 1024px) {
  .baseline {
    margin-top: 60px;
    margin-bottom: 70px;
  }

  .baseline_first {
    margin-left: -1300px;
  }

  .baseline_second {
    margin-left: -200px;
  }

  .baseline_first p {
    font-size: 80px;
    line-height: 80px;
  }

  .baseline_second p {
    font-size: 80px;
    line-height: 80px;
  }
}
</style>
