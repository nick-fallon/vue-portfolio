<template id="">
  <div>
    <v-app>
      <div class="main">
        <v-container>
          <header>
            <h1>{{ title }}</h1>
          </header>
          <v-layout>
            <v-flex xs12 offset-md2>
              <div v-for="project in projects" :key="project.title">
                <v-card class="my-4">
                  <v-card-media
                    class="white--text"
                    height="190px"
                    :src="project.image"
                  >
                  </v-card-media>
                  <v-card-title primary-title>
                    <div>
                      <h3 class="headline mb-0">{{ project.title }}</h3>
                      <div>{{ project.description }}</div>
                    </div>
                  </v-card-title>
                  <v-card-actions>
                    <a :href="project.siteUrl"><v-btn icon class="black--text">
                      <v-icon medium>fa-external-link</v-icon>
                    </v-btn></a>
                    <a :href="project.github"><v-btn icon class="black--text">
                      <v-icon medium>fa-github</v-icon>
                    </v-btn></a>
                    <v-spacer></v-spacer>
                    <v-btn flat class="blue--text">Read More</v-btn>
                  </v-card-actions>
                </v-card>
              </div>
            </v-flex>
          </v-layout>
        </v-container>
      </div>
    </v-app>
  </div>
</template>

<script type="text/javascript">
  export default {
    data() {
      return {
        title: 'Projects',
        projects: [
          {
            title: 'Plague Nation',
            description: 'Description of Plague Nation',
            image: 'http://res.cloudinary.com/dpcbzfiye/image/upload/v1465331820/v8jhrktzok3m7sowsagq.jpg',
            siteUrl: 'https://plague-nation-1499461518065.firebaseapp.com/#/',
            github: 'https://github.com/nickpfallon/plague-nation'
          },
          {
            title: 'Pixelaid',
            description: 'Description of Pixelaid',
            image: 'https://i.ytimg.com/vi/iQsnObyii4Q/maxresdefault.jpg',
            siteUrl: 'http://pixelaid.herokuapp.com/',
            github: 'https://github.com/Pixelaid-Team/Pixelaid'
          },
          {
            title: 'GrooveBass',
            description: 'Description of GrooveBass',
            image: 'http://images.adsttc.com/media/images/57cf/7e00/e58e/ce96/5700/00eb/large_jpg/the_Learning_Center_01.jpg?1473215991',
            siteUrl: 'https://www.youtube.com/watch?v=pY8IAGtAmU8',
            github: 'https://github.com/Groove-Bass/Groove-Bass-the-Repo'
          },
          {
            title: 'M\u00fcncher',
            description: 'Description of M\u00fcncher',
            image: 'https://cdn.pixabay.com/photo/2016/01/13/21/24/architecture-1138967_960_720.jpg',
            siteUrl: 'https://q1-project-943b7.firebaseapp.com/',
            github: 'https://github.com/nickpfallon/project-q1'
          }
        ]
      }
    }
  }
</script>

<style media="screen" scoped>
  .main {
    background-color: #006064;
    height: 100%;
  }
  h1 {
    color: #ffd24c;
  }
  header {
    display: flex;
    justify-content: center;
  }
  a {
    text-decoration: none;
  }
</style>
