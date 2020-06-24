<template>
  <v-img aspect-ratio="2" width="100%" :src="headerImg">
    <v-row align="center" style="height: 100%">
      <v-col>
        <v-row justify="center">
          <v-card-title class="page_title">
            上智大学ジャズ研究会
          </v-card-title>
        </v-row>
        <!-- <v-row class="mt-12" justify="center" align="baseline">
          <v-card-action>
            <v-btn class="scroll_button" text>
              <p>scroll</p>
              <v-row class="mt-2">
                <v-spacer />
                <v-img :src="require('~/assets/arrow.svg')" />
                <v-spacer />
              </v-row>
            </v-btn>
          </v-card-action>
        </v-row> -->
      </v-col>
    </v-row>
  </v-img>
</template>

<script>
export default {
  data: () => ({
    headerImg: require('~/assets/images/header_6.jpg')
  })
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@300&display=swap');

.page_title {
  font-family: 'Noto Serif JP', serif;
  font-size: 50px;
  border-bottom: 1px solid;
}

.scroll_button {
  font-family: 'Noto Serif JP', serif;
  font-size: 30px;
}

.arrow {
  // transform: scale(1, -1);
  // fill: white;
}
</style>
