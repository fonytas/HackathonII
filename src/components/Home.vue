<template>
  <v-container fluid>
    <v-layout row wrap>
      <!--<v-flex xs12 class="text-xs-center" mt-5>-->
        <!--<h1>Home page</h1>-->
      <!--</v-flex>-->
      <!--<v-flex xs12 class="text-xs-center" mt-3>-->
        <!--<p>This is a user's home page.</p>-->
      <!--</v-flex>-->

      <v-flex xs12 sm6 offset-sm3>
        <v-tabs icons-and-text centered dark color="primary">
          <v-tabs-slider color="secondary"></v-tabs-slider>
          <v-tab href="#tab-1">
            <v-icon color="secondary">arrow_drop_down</v-icon>
            First Trimester
          </v-tab>

          <v-tab href="#tab-2">
            <v-icon color="secondary">arrow_drop_down</v-icon>

            Second Trimester
            <!--<v-icon color="secondary">favorite</v-icon>-->
          </v-tab>
          <v-tab href="#tab-3">
            <v-icon color="secondary">arrow_drop_down</v-icon>
            Third Trimester
            <!--<v-icon color="secondary">account_box</v-icon>-->
          </v-tab>

          <v-tab href="#tab-4">
            <v-icon color="secondary">arrow_drop_down</v-icon>
            Summer
            <!--<v-icon color="secondary">account_box</v-icon>-->
          </v-tab>
          <v-tab-item
            v-for="i in 4"
            :key="i"
            :id="'tab-' + i"
          >
            <v-card flat>
              <v-card-text>{{ text }}</v-card-text>
            </v-card>
          </v-tab-item>
        </v-tabs>
      <!--<v-card>-->
        <!--<v-card-media src="/static/material.jpg" height="200px">-->
        <!--</v-card-media>-->
        <!--<v-card-title primary-title>-->
          <!--<div>-->
            <!--<h3 class="headline mb-0">Kangaroo Valley Safari</h3>-->
            <!--<div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>-->
          <!--</div>-->
        <!--</v-card-title>-->
        <!--<v-card-actions>-->
          <!--<v-btn flat color="orange">Share</v-btn>-->
          <!--<v-btn flat color="orange">Explore</v-btn>-->
        <!--</v-card-actions>-->
      <!--</v-card>-->
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      tabs: null,
      text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
    }
  }
}
</script>
