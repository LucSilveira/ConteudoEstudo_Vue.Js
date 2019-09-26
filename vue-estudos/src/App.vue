<template>
  <v-app id="inspire">
    <v-navigation-drawer fixed v-model="drawer" app>
      <v-list dense>
        <router-link v-bind:to="{ name: 'HelloWorld' }" class="side_bar_link"> 
          <v-list-tile>
            <v-list-tile-action>
              <v-icon>home</v-icon>
              </v-list-tile-action>
              <v-list-tile-content>Home</v-list-tile-content>
              </v-list-tile>
              </router-link>
              <router-link v-bind:to="{ name: 'Produtos' }" class="side_bar_link">
                <v-list-tile>
                  <v-list-tile-action>
                    <v-icon>contact_mail</v-icon>
                  </v-list-tile-action>
                  <v-list-tile-content>Produto</v-list-tile-content>
                  </v-list-tile>
                  </router-link>
                  </v-list>
                  </v-navigation-drawer>
                  <v-toolbar color="indigo" dark fixed app>
                    <v-toolbar-side-icon @click.stop="drawer = !drawer">
                      </v-toolbar-side-icon>
                      <v-toolbar-title>Home</v-toolbar-title>
                      </v-toolbar>
                      <v-content>
                        <v-container fluid>
                          <div id="app">
                            <router-view/>
                            </div>
                            </v-container>
                            </v-content>
                            <v-footer color="indigo" app>
                              <span class="white--text">&copy; 2018</span>
                              </v-footer>
                              </v-app>
</template>


<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  }
  
#inspire {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  } 
 
.container.fill-height {
  align-items: normal;
  } 
 
a.side_bar_link {
  text-decoration: none;
  } 
</style>


<!--div id="app">
    <img src="./assets/logo.png">
    <router-view/>
  </div>
<script>
export default {
  name: 'App',
};
</style>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>-->