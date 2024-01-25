<script setup>
const name = ref("NAWIGACJA");
</script>
<template>
  <link href='https://fonts.googleapis.com/css?family=Noto Sans KR' rel='stylesheet'>
  <nav>
    <div class="navbar">
      <div class="logos">
        <img src="./logo.png" alt="" />
        <div class="socialsDiv">
          <img src="./socials.png" alt="">
        </div>
      </div>
      <div class="menu">

        <NuxtLink to="/"><span>O NAS</span></NuxtLink>

        <nuxt-link to="/about"><span>BLOG</span></nuxt-link>
        <a href="/about"><span>OPINIE</span></a>
        <nuxt-link to="/articles/1"><span>KONTAKT</span></nuxt-link>

        <button>Zaloguj</button>


      </div>
    </div>
    <div class="line-1"></div>
  </nav>
</template>
<style scoped lang="scss">
h1 {
  color: red;
}

ul {
  .mpa {
    color: yellow
  }

}

img {
  width: 40%;

}

.navbar {
  display: flex;
  flex-direction: row;

  button {
    background-color: #DCA86F;
    border: none;
    color: white;
    font-size: 20px;
    font-weight: 700;
    position: relative;
    top: 30px;
    right: 20px;
    width: 170px;
    height: 50px;
    border-radius: 45px;
  }


}

span {

  position: relative;
  top: 110px;
  font-family: 'Noto Sans KR';

  a {
    text-decoration: none;

  }

  color: #6A6A6A;
  font-weight: 900;
  font-size: 24px;
  margin: 50px;
}

.line-1 {
  height: 39px;
  background: black;
  position: relative;
  top: -10px;
  z-index: 99;
}

.logos {
  width: 50%;

  display: flex;
  justify-content: center;
  align-self: center;

  .socialsDiv {
    width: 80%;
    display: flex;
    justify-content: center;
    align-self: center;
  }
}
</style>