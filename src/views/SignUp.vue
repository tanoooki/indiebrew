<template>
  <div class="background">

    <div class="menu_2">
      <img src="../assets/Logo.svg" alt="Logo IndieBrew">
      <div class="canto">
        <router-link to="/">
          <img class="detalhe_2" src="../assets/less.svg" alt="">
        </router-link>
          <router-link to="/">
          <p class="esconder_mobile"><b>Voltar para Home</b></p>
        </router-link>
      </div>
    </div>

    <div class="principal">
      <div>
        <h2>Crie seu feed personalizado.</h2>
        <div class="info">
          <p style='font-size:25px;'>&#x1F388;</p>
          <p><b>Mais de 20 recursos.</b> Com recursos vindo do Reddit para o IndieHackers, nós temos cobertura de tudo o
            que você precisa.</p>
        </div>
        <div class="info">
          <p style='font-size:25px;'>&#128240;</p>
          <p><b>Entrega semanal.</b> Toda semana exatamente as terças 12:00pm, receba em seu e-mail todo o conteúdo.</p>
        </div>
        <div class="info">
          <p style='font-size:25px;'>&#x1F4A1;</p>
          <p><b>Ideias ilimitadas.</b> Com todas a ideias que você lerá sobre, por quê parar de criar coisas novas?</p>
        </div>
      </div>

      <div class="formulario">
        <h3>Crie sua conta IndieBrew</h3>
        <label for="email">Email</label>
        <input type="email" name="email" id="email" placeholder="john@example.com">
        <label for="name">Nome Completo</label>
        <input type="text" name="name" id="name" placeholder="John Doe">
        <label for="password">Senha</label>
        <input type="password" name="password" id="password" placeholder="No mínimo 8 caracteres">
        <div class="termos">
          <input type="checkbox" id="si">
          <label for="si"></label>
          <span>Criando uma conta na IndieBrew, você aceita com os <span
              style="color: blue; text-decoration: underline; cursor: pointer"> Termos & Condições</span>.</span>
        </div>
        <button class="criar">Crie uma conta</button>
      </div>

    </div>
  </div>
</template>

<style>
.background {
  background: radial-gradient(circle, #f0def7 0%, #fdfcf9 90%);
  height: 100vh;
}

.menu_2 {
  display: flex;

  justify-content: space-between;
  padding: 40px 60px;
  max-width: 1200px;
  margin: 0 auto;
}

.canto {
  display: flex;
  gap: 10px;
  align-items: center;
}

.detalhe_2 {
  background: rgb(255, 255, 255, 0.4);
  border: 1px solid lightgray;
  padding: 10px 10px;
  color: #000;
  border-radius: 8px;
  max-width: 12px;
  max-height: 12px;
}

.principal {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
  text-align: start;
  max-width: 1000px;
  margin: 0 auto;
  padding: 40px 40px;
  text-align: justify;
  place-items: center;
}

.info {
  display: grid;
  grid-template-columns: 25px 1fr;
  gap: 20px;
  place-items: center;
}

.formulario {
  background: #fff;
  padding: 30px;
  border-radius: 8px;
  display: grid;

}

.formulario h3 {
  padding-bottom: 20px;
}

label {
  font-weight: bold;
  padding-bottom: 10px;
}

input {
  border-radius: 4px;
  border: 1px solid lightgray;
  font-size: 1rem;
  color: rgb(185, 185, 185);
  padding: 1rem;
  margin-bottom: 10px;
}

.termos {
  font-size: 0.9rem;
  padding: 10px 0px 30px 0px;

}

.termos label {
  margin-right: 6px;
}

.criar {
  padding: 15px 12px;
  background-color: #664efc;
  color: #fff;
  border-radius: 4px;
  border: none;
  font-size: 1.2rem;
  cursor: pointer;
}

.criar:hover {
  background-color: #4732cf;
}


@media (max-width: 700px) {
  .principal {
    grid-template-columns: 1fr;
  }
  .info {

  }
}

@media (max-width: 500px){
  .esconder_mobile {
    display: none;
  }
  .menu_2 {
    padding: 40px;
  }
}
</style>