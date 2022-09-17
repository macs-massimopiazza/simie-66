<template>
  <div id="app">
    <h1 style="color: green;">🥰Viva Classe 66🥰</h1>
    <h3>🐵🐒A cui a quanto pare piacciono le scimmie🐵🐒</h3>
    <span style="color: blue; background: white;">💕I vostri insegnanti e coordinatori: Luca, Alessandro, Paolo e Massimo 💕</span>
    <iframe style="border-radius:12px;" src="https://open.spotify.com/embed/track/6gxycjJNMgmAyfzUXBN80P?utm_source=generator" width="90%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
    <h1 style="color: greenyellow;">✨ Le vostre scimmie ✨</h1>
    <ul>
      <li v-for="(scimmia, index) in scimmie" :key="index"><img :src="scimmia.url" :alt="scimmia.alt"> <span>{{ scimmia.alt }}</span></li>
    </ul>

  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      scimmie: [
        { alt: "la scimmia triste di manuel", url: "https://pbs.twimg.com/media/FEhF3U1WQAAcXBT?format=jpg&name=large"},
        { alt: "la scimmia di edoard borr", url: "https://centerforgreatapes.org/wp-content/uploads/2021/03/IMG_00251_Louie.jpg"},
        { alt: "la scimmia di lucio", url: "https://i2.wp.com/www.linkiesta.it/wp-content/uploads/2020/02/dd998222-599c-4aa4-a8b4-49f0feaf1268_large.jpg?fit=1200,874&ssl=1"},
        { alt: "la seconda scimmia di lucio", url: "https://media.npr.org/assets/img/2017/09/12/macaca_nigra_self-portrait-3e0070aa19a7fe36e802253048411a38f14a79f8-s1100-c50.jpg"},
        { alt: "la scimmia di edomndo", url: "https://media-assets.wired.it/photos/615c496336911c2d72f97331/master/pass/1415182318_2001_a_space_odyssey_scimmia.jpg"},
        { alt: "la scimmia di davide che è uguale a quella di lucio", url: "https://media.npr.org/assets/img/2017/09/12/macaca_nigra_self-portrait-3e0070aa19a7fe36e802253048411a38f14a79f8-s1100-c50.jpg"},
        { alt: "la scimmia di andrei", url: "https://www.marcotogni.it/v-2/34/jigokudani.jpg"},
        { alt: "la scimmia di vincenzo", url: "https://1.bp.blogspot.com/-uKONCFlu-NE/UP63qo4kXqI/AAAAAAAAONA/QS46Dbk91kQ/s1600/immagini+divertenti+di+scimmie+2.jpg"},
        { alt: "la scimmia cattiva di lorenzo", url: "https://nerdmovieproductions.it/wp-content/uploads/2021/02/godzilla-770x488.jpg"},
        { alt: "la scimmia di lisa", url: "https://media-assets.wired.it/photos/615f078b4c30266a0d6379dd/master/w_960,c_limit/1481626523_scimmie-em.jpg"},
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  background-color:rgb(255, 72, 0);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
 
}

li {
  position: relative;
  width: fit-content;
  margin: 0 auto;
  list-style-type: none;
  font-size: 20px;
  margin-bottom: 5px
}

li span {
  position: absolute;
  top: 10px;
  left: 10px;
  background-color: #fff;
  color: black;
} 

img {
  width: 600px;
}

h1, h3, img, p, ul {
  margin-bottom: 20px;
}
</style>
