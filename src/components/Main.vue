<template id="">
  <div>
    <v-app>
      <div class="main-container cyan darken-4">
        <div class="name-container">
          <h1>Nick Fallon</h1>
          <nav>
            <ul class="sub-nav">
              <router-link to="/about"><li><a>About Me</a></li></router-link>
              <router-link to="/projects"><li><a>Projects</a></li></router-link>
              <li><a>Resume</a></li>
              <router-link to="/contact"><li><a>Contact Me</a></li></router-link>
            </ul>
          </nav>
        </div>
      </div>
    </v-app>
  </div>
</template>

<script type="text/javascript">

</script>

<style media="screen" scoped>
  .main-container {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
  }
  .sub-nav {
    padding: 0;
    font-size: 1.5em;
    margin-top: 2em;
    list-style-type: none;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }
  a {
    text-decoration: none;
    color: #fff;
  }
  h1 {
    margin: 0;
    color: #ffd24c;
  }
</style>
