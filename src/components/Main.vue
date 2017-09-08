<template id="">
  <div>
    <v-app>
      <div class="main-container cyan darken-4">
        <div class="name-container">
          <h1>Nick Fallon</h1>
          <nav>
            <div class="sub-nav">
              <p>Full Stack Developer</p>
            </div>
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
    margin-top: 1em;
    color: white;
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
