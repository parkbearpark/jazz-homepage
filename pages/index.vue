<template>
  <div>
    <Header />
    <v-container>
      <v-layout column justify-center align-center>
        <!-- About -->
        <v-row style="width: 100%">
          <v-card flat>
            <v-row justify="center">
              <v-card-subtitle class="subtitle">About</v-card-subtitle>
            </v-row>
            <v-card-text
              >上智大学ジャズ研究会は上智大学のジャズ研究会。<br />
              部員約60名。他大生も多数在籍しております。<br />
              週一回のセッションと２ヶ月に１回の演奏会を<br />
              主な活動としています。</v-card-text
            >
          </v-card>
        </v-row>
        <!-- About -->

        <!-- Activities -->
        <v-row justify="center" style="width: 100%">
          <v-card flat>
            <v-row justify="center">
              <v-card-subtitle class="subtitle">Activities</v-card-subtitle>
            </v-row>
            <v-card-text
              >上智ジャズ研では週１回のセッションと2ヶ月に1
              回の演奏会を主な活動としています。</v-card-text
            >
            <v-data-table
              :headers="activityHeaders"
              :items="activities"
              :items-per-page="5"
              hide-default-footer
            >
            </v-data-table>
          </v-card>
        </v-row>
        <!-- Activities -->
      </v-layout>
    </v-container>
  </div>
</template>

<script>
import Header from '~/components/Header'

export default {
  components: {
    Header
  },
  data: () => ({
    activityHeaders: [{ value: 'date' }, { value: 'time' }, { value: 'name' }],
    activities: [
      {
        date: '2019.12.23',
        time: '11:00~16:00',
        name: 'クリスマスコンサート@SBC'
      },
      {
        date: '2019.12.23',
        time: '11:00~16:00',
        name: 'クリスマスコンサート@SBC'
      },
      {
        date: '2019.12.23',
        time: '11:00~16:00',
        name: 'クリスマスコンサート@SBC'
      }
    ]
  })
}
</script>

<style lang="scss" scoped>
.subtitle {
  font-family: 'Noto Serif JP', serif;
  font-size: 50px;
  border-bottom: 1px solid;
  text-align: center;
}
</style>
