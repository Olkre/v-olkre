<template>
  <div id="app">
    <block1 />
    <div class="container b2" id="projects">
      <div class="b2-title-cont">
        <h3 class="b2-title">Projects</h3>
      </div>
      <section class="projects row">
        <Card
        v-for="card in projects"
        :key="card.iden"
        :card="card"
        />
    </section>
    </div>
    <vfooter />
  
  </div>
</template>

<script>
import Card from './components/Card'
import Vfooter from './components/Vfooter'
import Block1 from './components/b1'
export default {
  name: 'App',
  components: {
    Card,
    Vfooter,
    Block1
  },
  data() {
    return {
      projects: [
        // {
        //   title: 'Pomodoro Countdown Time',
        //   desc: 'Mobile App / Dribbble',
        //   src: require('./assets/Projects/timer.png'),
        //   link: 'https://dribbble.com/shots/13644575-Countdown-Timer-DailyUI-014',
        //   iden: '4'
          
        // },
        {
          title: 'Providence Bicycle Bike shop',
          desc: 'Web Site / Behance',
          src: require('./assets/Projects/bike.png'),
          link: 'https://www.behance.net/gallery/92691161/Providence-Bicycle-website-for-a-bike-shop',
          iden: '3'
        },
        {
          title: 'AirPods Max - Control App',
          desc: 'Mobile App / Dribbble',
          src: require('./assets/Projects/airpods.png'),
          link: 'https://dribbble.com/shots/14781247-AirPods-Max-Control-App',
          iden: '2'
        },
        {
          title: 'Pop Up with 3D icons',
          desc: '3D / Mobile App /  Web / Dribbble',
          src: require('./assets/Projects/popup.png'),
          link: 'https://dribbble.com/shots/13827069-Pop-Up-with-3d-icons-Daily-UI-016',
          iden: '1'
        }
      ]
    }
  }
}
</script>

<style>
  @import 'styles/styles.css';
</style>
