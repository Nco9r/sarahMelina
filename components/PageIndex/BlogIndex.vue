<template>
  <section class="blog">
    <div class="title_blog">
      <h3><span>FoodMag</span></h3>
    </div>
    <div class="items_blog">
      <no-ssr>
        <vue-tiny-slider v-bind="tinySliderOptions" ref="tinySlider">
          <div class="item">
            <img src="~/assets/img/jpg/projets_1.jpg" alt="" />
            <p class="title_item">Comment optimiser une photo culinaire</p>
            <p class="sous_title">Le 27/02/2022 par Sarah Melina</p>
            <p class="infos">
              Pour améliorer et réussir ses photos culinaires, il existe une
              règle simple pour commencer : privilégier la lumière naturelle du
              jour, sans flash, qui donne une lumière trop artificielle et
              brutale
            </p>
            <p class="suite">Lire la suite</p>
          </div>
           <div class="item">
            <img src="~/assets/img/jpg/projets_1.jpg" alt="" />
            <p class="title_item">Comment optimiser une photo culinaire</p>
            <p class="sous_title">Le 27/02/2022 par Sarah Melina</p>
            <p class="infos">
              Pour améliorer et réussir ses photos culinaires, il existe une
              règle simple pour commencer : privilégier la lumière naturelle du
              jour, sans flash, qui donne une lumière trop artificielle et
              brutale
            </p>
            <p class="suite">Lire la suite</p>
          </div>
        </vue-tiny-slider>
      </no-ssr>
    </div>
    <div class="btn">
      <button>Toutes les actus</button>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      tinySliderOptions: {
        mouseDrag: true,
        loop: true,
        items: 1,
        nav: false,
        container: '.box_cards',
        autoplayButtonOutput: false,
        gutter: 80,
        autoplayTimeout: 5000,
        autoplay: true,
        speed: 800,
        preventScrollOnTouch: 'auto',
        controls: true,
        prevButton: '#prev_p',
        nextButton: '#next_p',
        responsive: {
          1024: {
            items: 3,
            edgePadding: 40,
            loop: false,
            prevButton: '#prev_c',
            nextButton: '#next_c',
          },
        },
      },
    }
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href: 'https://cdnjs.cloudflare.com/ajax/libs/tiny-slider/2.9.1/tiny-slider.css',
        },
      ],
    }
  },
}
</script>

<style scoped>
span {
  background-color: var(--yellow);
}

.blog {
  margin-top: -100px;
  padding: 0 15px;
  margin-bottom: 80px;

}

.title_blog h3 {
  font-size: 28px;
  font-weight: 900;
}

.title_blog {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.items_blog {
  margin-top: 30px;
}

.item img {
  width: 100%;
  height: 250px;
  object-fit: cover;
  border-radius: 6px;
}

.title_item {
  margin-top: 20px;
  font-size: 22px;
  font-weight: 900;
}
.sous_title {
  margin-top: 10px;
  text-transform: uppercase;
  font-size: 12px;
  color: var(--gray-secondary);
  font-weight: 900;
}

.infos {
  margin-top: 15px;
  color: var(--body);
  line-height: 26px;
}

.suite {
  font-weight: 900;
  margin-top: 15px;
}

.tns-nav {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100px;
  margin: auto;
}

.tns-nav button {
  border: 1px solid var(--gray);
  background-color: transparent;
  margin-right: 10px;
  height: 14px;
  width: 14px;
  border-radius: 50%;
}

.btn button {
  display: flex;
  margin: 60px auto;
  background-color: var(--yellow);
}
</style>
