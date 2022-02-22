<template>
  <footer>
    <div class="box_footer">
      <div class="box_newsletter">
        <div class="title_news">
          <h4>INSCRIPTION À LA NEWSLETTER</h4>
          <p>
            Vous souhaitez recevoir des nouvelles actualités ou recettes
            inédites ? Ça se passe ici.
          </p>
        </div>
        <div class="input">
          <input
            type="email"
            placeholder="votre@email.fr ici"
            v-model="newsletter"
          />
          <button :class="{ valide: newsletter.length > 1 }">Soumettre</button>
        </div>
      </div>
      <div class="box_items_footer">
        <div class="item">
          <h5>Plan du site</h5>
          <p>Services</p>
          <p>Réalisations</p>
          <p>FoodMag</p>
        </div>
        <div class="item">
          <h5>INFORMATIONS LÉGALES</h5>
          <p>Contact</p>
          <p>Mentions légales</p>
          <p>Politique de confidentialité</p>
        </div>
        <div class="item">
          <h5>Contact</h5>
          <p>foodpreneur@sarahmelina.com</p>
          <p>+33 (0)6 00 00 00 00</p>
          <p>
            5 bis Place du souvenir, <br />
            33610, Cestas, FRANCE
          </p>
        </div>
      </div>
      <div class="box_sociaux">
          <div class="item">
              <h5>Réseaux sociaux</h5>
              <div class="box_logo_sociaux">
                  <img src="~assets/img/svg/fb_bis.svg" alt="">
                  <img src="~assets/img/svg/insta_bis.svg" alt="">
                  <img src="~assets/img/svg/lin_bis.svg" alt="">
              </div>
          </div>
      </div>
      <div class="copyright">
          <p>©2022 - by_sarahmelina tous droits réservés.</p>
          <p>Made by Nicolas ROUX</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      newsletter: '',
    }
  },
}
</script>

<style scoped>
footer {
  background-color: var(--rose);
 padding-bottom: 30px;
}

.box_newsletter {
  display: flex;
  flex-flow: column;
  padding: 50px 15px;
}

.title_news h4 {
  font-weight: 900;
  font-size: 22px;
}

.title_news p {
  margin-top: 10px;
  line-height: 24px;
}

.input {
  margin-top: 30px;
}

.input input {
  background-color: transparent;
  border: none;
  background-image: url('~assets/img/svg/next.svg');
  background-repeat: no-repeat;
  background-position: 95% 50%;
  background-size: 8%;
  padding: 20px;
  outline: none;
  font-size: 16px;
  width: 100%;
  border-bottom: 1px solid var(--black);
}

.input input::placeholder {
  color: var(--black);
  font-family: 'Lato', sans-serif;
}

.input button {
  background-color: #fce7ea;
  border: none;
  padding: 16px 20px;
  width: 170px;
  margin-top: 15px;
  float: right;
  font-weight: 900;
  color: var(--gray-secondary);
  transition: all 0.3s;
}

.valide {
  background-color: var(--white) !important;
  color: var(--black) !important;
}

.box_items_footer {
  padding: 0 15px;
  display: flex;
  flex-flow: row wrap;
}

.item {
  width: 170px;
  margin-bottom: 20px;
}

.item h5 {
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 900;
  margin-bottom: 10px;
}

.item p {
  margin-bottom: 10px;
}

.box_sociaux {
padding: 0 15px;
}

.box_logo_sociaux {
    margin-top: 20px;
}

.copyright {
    padding: 0 15px;
    margin-top: 40px;
}

.copyright p {
    margin-bottom: 10px;
}
</style>
