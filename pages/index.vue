<template>
  <main class="attente">
    <div class="hero_content">
    <div class="logo">
      <img src="~assets/img/svg/logo_S.svg" alt="" />
    </div>

    <div class="content_hero">
      <h1>By Sarah Melina évolue !</h1>
      <p>
        Le site est en cours de reconstruction pour vous proposer une meilleure
        expérience de navigation, et encore plus de douceurs culinaires. En
        attendant, contactez-moi sur les réseaux !
      </p>
      <a href="https://www.facebook.com/bysarahmelina/" target="_blank">
      <img src="~assets/img/svg/fb.svg" alt="">
      </a>
       <a href="https://www.instagram.com/by_sarahmelina/?hl=fr" target="_blank">
      <img src="~assets/img/svg/insta.svg" alt="">
      </a> <a href="https://fr.linkedin.com/in/sarah-da-silva-94823017b" target="_blank">
      <img src="~assets/img/svg/lin.svg" alt="">
      </a>
    </div>
    </div>
  </main>
</template>

<script>
export default {}
</script>

<style scoped>
main {
  width: 100%;
  height: 100vh;
  background-image: url('~assets/img/jpg/hero_img3.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-flow: column;
  align-items: flex-end;
  justify-content: center;
  background-position: 60%;
 
}

.hero_content {
  margin-top: -00px;
}

.attente {
  text-align: center;
}

.content_hero {
  margin-top: -50px;

}

.content_hero h1 {
  font-size: 26px;
  margin-bottom: 10px;
}

.content_hero p {
  padding: 5px 5px;
  font-size: 14px;
  margin: auto;
  width: 360px;
  line-height: 22px;
  color: rgb(78, 78, 78);
}

.content_hero img {
  margin-top: 20px;
}

@media screen and (min-width: 1024px) {
.attente {
  text-align: center;
 
}

.hero_content {
  margin-right: 50px;

}


.content_hero h1 {
  font-size: 36px;
  margin-bottom: 20px;
}


.content_hero p {
  padding: 15px 5px;
  font-size: 18px;
  width: 500px;
  line-height: 32px;
  color: rgb(78, 78, 78);
}

  
}

@media screen and (min-width: 1200px) {
.attente {
  text-align: center;
 
}

.hero_content {
  margin-right: 50px;

}


.content_hero h1 {
  font-size: 36px;
  margin-bottom: 20px;
}


.content_hero p {
  padding: 15px 5px;
  font-size: 18px;
  width: 600px;
  line-height: 32px;
  color: rgb(78, 78, 78);
}

  
}

@media screen and (min-width: 1600px) {
.attente {
  text-align: center;
 
}

.hero_content {
  margin-right: 200px;

}


.content_hero h1 {
  font-size: 46px;
  margin-bottom: 20px;
}


.content_hero p {
  padding: 15px 5px;
  font-size: 22px;
  width: 750px;
  line-height: 36px;
  color: rgb(78, 78, 78);
}

  
}

</style>
