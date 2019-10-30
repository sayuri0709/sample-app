<template>
  <v-container text-xs-center justify-center>
    <v-layout row wrap>
      <v-flex xs12>
        <h1>アドレス帳に連絡先を追加できます</h1>
        <p>※追加された連絡先はリロードすると消去されます。</p>
      </v-flex>

      <v-flex xs12 mt-4 justify-center>
          <router-link :to="{name: 'address_edit'}">
              <v-btn color="info">連絡先追加</v-btn>
          </router-link>
      </v-flex>

    </v-layout>
  </v-container>
</template>

<script>
  export default {
  }
</script>
<style>
  h1 + p {
    margin-top: 10px;
  }
</style>