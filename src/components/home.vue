<template>
  <div class="home">
    <h1>Video Games</h1>
    <div class="row">
      <div class="col-md-4 col-lg4" v-for="(data,index) in games" :key="index">
        <img :src="data.image" class="img-fluid" :alt="data.title">
        <h3>{{data.title}}</h3>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Home',
  data () {
    return {
      listTitle: 'List of Video Games',
      games: [
        {
          title: 'The Last of Us',
          image: '',
          yearOfRelease: 2013
        },
        {
          title: 'Metal Gear Solid',
          image: '',
          yearOfRelease: 1998
        },
        {
          title: 'The Legend of Zelda: Ocarina of Time',
          image: '',
          yearOfRelease: 1998
        },
        {
          title: 'Grand Theft Auto V',
          image: '',
          yearOfRelease: 2013
        },
        {
          title: 'Max Payne',
          image: '',
          yearOfRelease: 2001
        },
        {
          title: 'Resident Evil',
          image: '',
          yearOfRelease: 2002
        },
        {
          title: 'Halo: Combat Evolved',
          image: '',
          yearOfRelease: 2001
        },
        {
          title: 'God of War',
          image: '',
          yearOfRelease: 2005
        },
        {
          title: 'Uncharted 4: A Thief\'s End',
          image: '',
          yearOfRelease: 2016
        },
        {
          title: 'Prince of Persia: The Sands of Time',
          image: '',
          yearOfRelease: 2003
        },
      ]
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>