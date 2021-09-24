<template>
  <div>
    <h1>{{ titulo }}</h1>
    <url>
      <li v-for="foto of fotos">
        <img :src="foto.url" :alt="foto.titulo" />
      </li>
    </url>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      titulo: "Cachorro",
      fotos: [
        {
          url: "https://s2.glbimg.com/slaVZgTF5Nz8RWqGrHRJf0H1PMQ=/0x0:800x450/984x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_59edd422c0c84a879bd37670ae4f538a/internal_photos/bs/2019/U/e/NTegqdSe6SoBAoQDjKZA/cachorro.jpg",
          titulo: "cachorro",
        },
        {
          url: "https://s2.glbimg.com/slaVZgTF5Nz8RWqGrHRJf0H1PMQ=/0x0:800x450/984x0/smart/filters:strip_icc()/i.s3.glbimg.com/v1/AUTH_59edd422c0c84a879bd37670ae4f538a/internal_photos/bs/2019/U/e/NTegqdSe6SoBAoQDjKZA/cachorro.jpg",
          titulo: "cachorro",
        },
      ],
    };
  },
  created(){
    alert('inicializando a aplicação')
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
