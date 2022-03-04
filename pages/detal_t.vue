<template>
  <div>
    <div class="h">
      <v-row>
        <v-col class="h1">
          <v-btn icon>
            <v-icon>mdi-account-circle</v-icon>
          </v-btn>
        </v-col>
        <v-col class="h2">
          <v-btn icon href="/">
            <v-icon>mdi-export</v-icon>
          </v-btn>
        </v-col>
      </v-row>
    </div><br>

    <div class="h  white">
      <h1 class="t">
        ข้อมูลผู้ประกอบการ
      </h1>
      <div class="h2 cyan lighten-3">
        <br><br><br><h3 class="t">
          บริษัท ไทยแลนด์ จำกัด
        </h3>
        <v-sheet
          class="h"
          color="indigo darken-4"
          elevation="1"
          height="50"
          outlined
          rounded
          width="330"
        >
          <h3 class="y">
            ข้อมูล
          </h3>
        </v-sheet><br>
        <v-row>
          <v-col md="6">
            <img src="@/assets/img/ca.jpg" width="30%">
          </v-col>
          <v-col md="3">
            <h4 class="t">
              05*********
            </h4>
          </v-col>
        </v-row>
        <v-row>
          <v-col md="6">
            <img src="@/assets/img/fa.png" width="30%">
          </v-col>
          <v-col md="3">
            <h4 class="t">
              **********
            </h4>
          </v-col>
        </v-row>
        <v-row>
          <v-col md="6">
            <img src="@/assets/img/emm.png" width="30%">
          </v-col>
          <v-col md="3">
            <h4 class="t">
              pyh****@gmail.com
            </h4>
          </v-col>
        </v-row>
        <br><br>
      </div>
      <br>
      <br><br>  <br><br>
    </div>
    <br><br>
  </div>
</template>
<style>
.t{
  color: black;
}
.h{
  text-align: center;
}
.y{
  margin: 3%;
}
</style>
