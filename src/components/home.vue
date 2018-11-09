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
          image: require('../assets/the_last_of_us_cover.png'),
          yearOfRelease: 2013
        },
        {
          title: 'Metal Gear Solid',
          image: require('../assets/metal_gear_solid_art.jpg'),
          yearOfRelease: 1998
        },
        {
          title: 'The Legend of Zelda: Ocarina of Time',
          image: require('../assets/The Legend of Zelda_ Ocarina of Time_cover.jpg'),
          yearOfRelease: 1998
        },
        {
          title: 'Grand Theft Auto V',
          image: require('../assets/gtav_cover.jpg'),
          yearOfRelease: 2013
        },
        {
          title: 'Max Payne',
          image: require('../assets/max_payne_art.jpg'),
          yearOfRelease: 2001
        },
        {
          title: 'Resident Evil',
          image: require('../assets/220px-Resident_Evil_2002_cover.jpg'),
          yearOfRelease: 2002
        },
        {
          title: 'Halo: Combat Evolved',
          image: require('../assets/halo_cover.jpg'),
          yearOfRelease: 2001
        },
        {
          title: 'God of War',
          image: require('../assets/god_of_war_ps2.png'),
          yearOfRelease: 2005
        },
        {
          title: 'Uncharted 4: A Thief\'s End',
          image: require('../assets/uncharted4_cover.jpg'),
          yearOfRelease: 2016
        },
        {
          title: 'Prince of Persia: The Sands of Time',
          image: require('../assets/220px-Sands_of_time_cover.jpg'),
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