<template id="">
  <div id="about">
    <v-app>
      <div class="container">
        <div class="main-container">
          <img src="../../static/avatar.png" alt="">
          <h1>about me</h1>
          <section>
            <p>My name is Nick Fallon (my friends like to call me by my last name because "Nick" is so common). I am a full-stack software developer.  I received a BA in Quantitative Economics with a minor in Mathematics from the University of Colorado Boulder in 2015. I worked in restaurants during high school and college. After college, I realized that a career in a purely financial discipline wasn't exactly what I wanted. I wanted to do something that would allow more of my creativity to shine through.</p>

            <p>I completed the Galvanize Web Development Immersive program in Denver, CO, because I wanted to accelerate my learning and gain the skills to work as a front-end, back-end, or full-stack web developer. I love software development because it allows me to unite my creativity with technology.  I am passionate about math and art and really enjoy finding interesting ways to combine the two.</p>
          </section>
          <h3>skills</h3>
          <div class="text-xs-center skill-container">
            <v-chip v-for="skill in skills" :key="skill.title">
              <v-avatar class="cyan darken-4">{{ skill.letter }}</v-avatar>
              {{ skill.title }}
            </v-chip>
          </div>
        </div>
      </div>
    </v-app>
  </div>
</template>

<script type="text/javascript">
export default {
  name: 'about',
  data () {
    return {
      skills: [
        { title: 'JavaScript', letter: 'J' },
        { title: 'CSS3', letter: 'C' },
        { title: 'HTML5', letter: 'H' },
        { title: 'Node.js', letter: 'N' },
        { title: 'jQuery', letter: 'J' },
        { title: 'Vue.js', letter: 'V' },
        { title: 'PostgreSQL', letter: 'P' },
        { title: 'Express', letter: 'E' },
        { title: 'Knex.js', letter: 'K' },
        { title: 'AJAX', letter: 'A' },
        { title: 'Mocha', letter: 'M' },
        { title: 'Bootstrap', letter: 'B' },
        { title: 'Materialize', letter: 'M' },
        { title: 'Handlebars', letter: 'H' },
        { title: 'React Native', letter: 'R' },
        { title: 'AngularJS 1.x', letter: 'A' },
        { title: 'REST', letter: 'R' },
        { title: 'Git + GitHub', letter: 'G' },
      ]
    }
  }
}

</script>

<style media="screen" scoped>
  .main-container {
    margin-left: 4em;
    margin-right: 4em;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  h1 {
    color: #006064;
    font-size: 4em;
    margin-top: 1em;
  }
  section {
    margin-top: 1.25em;
    margin-bottom: 1.25em;
    font-size: 1.25em;
  }
  h3 {
    color: #006064;
    margin-bottom: .75em;
  }
  img {
    margin-top: 3em;
    width: 200px;
    border: solid 4px #006064;
    border-radius: 50%;
  }
</style>
