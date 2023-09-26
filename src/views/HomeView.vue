<template>
  <div class="first_background">
    <div class="menu">
      <img src="../assets/Logo.svg" alt="IndieBrew Logo">
      <div>
        <a href="/">Preço</a>
        <a href="/">Suporte</a>
        <router-link to="/signup" class="button">Inscreva-se<span> — é grátis</span></router-link>
      </div>
    </div>

    <div class="menu_mobile">
      <img src="../assets/Logo.svg" alt="IndieBrew Logo">

      <img src="../assets/HamburgerMenu.svg" alt="">
    </div>



    <div class="oferta_grid">
      <div class="oferta_info">
        <h1>Seu resumo <br> Semanal de feed pessoal.</h1>
        <p>Com o IndieBrew, tenha feeds pessoais sobre recursos de toda a web, incluindo Reddit, HackerNews,
          IndieHackers e muito mais.</p>

        <router-link to="/signup" class="button">Inscreva-se<span> — é grátis</span></router-link>
        <img class="users" src="../assets/UserAvatars.svg" alt="usuários">
        <span>Junte-se com <span class="detalhe">32,642 </span>IndieBrewers neste feed pessoal.</span>
      </div>
      <img class="tablet" src="../assets/FeedMockup.png" alt="Tablet">
    </div>
  </div>

  <div class="grid_social_medias">
    <div>
      <h2>Selecione seu feed a partir de dezenas de recursos.</h2>
      <span>cobrimos todas as principais plataformas de onde alguém poderia querer fazer a curadoria de seu feed. Reddit,
        Product Hunt, Indie Hackers e muito mais.</span>
      <p>Veja a lista completa de recursos →</p>
    </div>
    <img src="../assets/SocialMediaIcons.png" alt="social media">
  </div>

  <div class="grid_social_medias_2">
    <img src="../assets/PhoneMockup.png" alt="cellphone">
    <div>
      <h2>Acesse seu feed do conforto do seu telefone.</h2>
      <span>Com aplicações nativas tanto para iOS quanto Android, acesse o conteúdo de forma fácil.</span>
      <p>Inscreva-se para a Lista de Espera →</p>
    </div>
  </div>
  <div class="second_background">

    <div class="footer">
      <div class="footer_info">
        <h3>IndieBrew</h3>
        <span>Com o IndieBrew, tenha feeds pessoais sobre recursos de toda a web, incluindo Reddit, HackerNews,
          IndieHackers e muito mais.</span>
        <p>Feito com ❤ no BR.</p>
      </div>
      <div class="footer_info_2">
        <div>
          <h3>Mapa do Site</h3>
          <a href="/">Home</a>
          <a href="/">Preços</a>
        </div>
        <div>
          <h3>Recursos</h3>
          <a href="/">Suporte</a>
          <a href="/">Contato</a>
          <a href="/">FAQ</a>
        </div>
        <div>
          <h3>Empresa</h3>
          <a href="/">Sobre</a>
          <a href="/">Suporte</a>
          <a href="/">Blog</a>
        </div>
        <div>
          <h3>Portfólios</h3>
          <a href="/">HackerNews</a>
          <a href="/">Reddit</a>
          <a href="/">Twitter</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'HomeView',
  components: {

  }
}
</script>

<style>
body,
a,
nav,
li,
ul,
h1,
h2,
h3,
h4 {
  margin: 0px;
  padding: 0px;
  text-decoration: none;
  color: #000;
  list-style-type: none;
}

.menu_mobile {
  display: none;
}

.first_background {
  background: radial-gradient(circle at 0% 0%, #ebcbf7 0%, #fdfcf9 20%)
}

.second_background {
  background-color: #fdfcf9;
}

.button:hover {
  background-color: #000;
}

.menu {
  display: flex;
  justify-content: space-between;
  padding: 40px 60px;
  max-width: 1200px;
  margin: 0 auto;
}

.menu a {
  padding: 15px 12px;
  margin-left: 20px;
}

.button {
  background-color: #664efc;
  color: #fff;
  border-radius: 4px;
}

.button span {
  color: #eeeffe;
}

.oferta_grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  padding: 80px 60px;
  max-width: 1200px;
  margin: 0 auto;
}

.oferta_info {
  text-align: start;
  display: grid;
}

.oferta_info h1 {
  font-size: 3rem;
  margin-bottom: 20px;
}

.oferta_info p {
  color: #6b6b6b;
}

.button {
  padding: 15px 12px;
  background-color: #664efc;
  color: #fff;
  border-radius: 4px;
  text-align: center;
  max-width: 170px;
  max-height: 20px;
}

.button span {
  color: #eeeffe;
}

.tablet {
  max-width: 100%;

}

.detalhe {
  color: #4c42fb;
  font-weight: bold;
}

.grid_social_medias p,
.grid_social_medias_2 p {
  color: #664efc;
  font-weight: bold;
  cursor: pointer;
}

.grid_social_medias {
  display: grid;
  grid-template-columns: 1.2fr 0.8fr;
  padding: 60px 60px;
  text-align: start;
}

.grid_social_medias img {
  max-width: 80%;
  align-self: center;
  justify-self: end;
}

.grid_social_medias_2 {
  display: grid;
  grid-template-columns: .8fr 1.2fr;
  text-align: start;
  align-items: center;
  padding: 0px 60px 60px 60px;
}

.grid_social_medias_2 img {
  max-width: 100%;
}

.grid_social_medias h2,
.grid_social_medias_2 h2 {
  font-size: 2rem;
}

.grid_social_medias,
.grid_social_medias_2 {
  max-width: 1200px;
  margin: 0 auto;
}

.footer {
  display: grid;
  grid-template-columns: 1fr 1fr;
  max-width: 1200px;
  margin: 0 auto;
  padding: 60px 60px;
  text-align: start;
  gap: 40px;
}

.footer_info_2 {
  display: flex;
  gap: 40px;
  flex-wrap: wrap;
  justify-content: space-between;
}

.footer h3 {
  margin-bottom: 20px;
}

.footer span {
  line-height: 25px;
}

.footer a {
  display: block;
  line-height: 25px;
}


@media (max-width: 1000px) {
  .oferta_grid {
    grid-template-columns: 1fr;
  }

  .tablet {
    max-width: 80%;
    padding-bottom: 20px;
    margin: 0 auto;
  }

  .oferta_info {
    grid-row: 2;
  }

  .users {
    padding-bottom: 20px;
    padding-top: 20px;
  }
}

@media (max-width: 666px) {
  .menu {
    display: none;
  }

  .menu_mobile {
    display: flex;
    justify-content: space-between;
    padding-bottom: 60px;
    padding: 20px;
  }

}
</style>