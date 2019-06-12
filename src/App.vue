<template>
  <div id="app">
    <ul>
      <li v-for="(foto, index) of fotos">
        <h1>{{titulo + ' ' + (index+1)}}</h1>
        <img :src="foto.url" :titulo="foto.titulo">
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      titulo: "Dog",
      fotos: [
        {
          url:
            "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTwV4kVzT5McBdGSgqlVeRzubrNH_mOrrkKseDOGFURq20HmsrelEfMU7It",
          titulo: "cachorro"
        },
        {
          url:
            "https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcTwV4kVzT5McBdGSgqlVeRzubrNH_mOrrkKseDOGFURq20HmsrelEfMU7It",
          titulo: "cachorro"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
</style>
