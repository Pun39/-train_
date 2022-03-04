<template>
  <div>
    <div class="ca">
      <h3>ขั้นตอนการยื่นเรื่องฝึกประสบการณ์วิชาชีพ</h3>
    </div>
    <div class="detal">
      <br>
      <v-row>
        <v-col md="6">
          <h4 class="j">
            1.เข้าสู่ระบบ/ลงทะเบียนใหม่
          </h4>
          <div class="j2">
            Login เข้าสู่ระบบ <br>
            หรือ ลงทะเบียนใหม่<br>
          </div>
        </v-col>
        <v-col>
          <img src="@/assets/img/user.png" width="80" height="80">
        </v-col>
      </v-row>
      <!---1---->

      <v-row>
        <v-col md="3">
          <img src="@/assets/img/map.png" width="100" height="80">
        </v-col>
        <v-col md="8">
          <div class="h1">
            2) ค้นหาสถานที่ฝึกงาน <br>
            ค้นหาข้อมูล <br>
            สถานที่ฝึกงานแยก <br>
            ตามภาคและจังหวัด
          </div>
        </v-col>
      </v-row>
      <!---2---->
      <v-row>
        <v-col md="6">
          <h4 class="j3">
            3) ขออนุมัติฝึกประสบการณ์วิชาชีพ
          </h4>
          <div class="j2">
            แจ้งความประสงค์ <br> เพื่อขอยื่น<br>
            ฝึกประสบการณ์ <br> วิชาชีพ <br>
          </div>
        </v-col>
        <v-col>
          <img src="@/assets/img/pa.png" width="100" height="80">
        </v-col>
      </v-row>
      <!---3---->
      <v-row>
        <v-col md="3">
          <img src="@/assets/img/ch.png" width="100" height="80">
        </v-col>
        <v-col md="8">
          <div class="h1">
            2) ค้นหาสถานที่ฝึกงาน <br>
            ค้นหาข้อมูล <br>
            สถานที่ฝึกงานแยก <br>
            ตามภาคและจังหวัด
          </div>
        </v-col>
      </v-row><br>
      <div class="btn">
        <v-btn href="/login" light>
          <h3>ถัดไป >></h3>
        </v-btn>
      </div>
      <!---4---->
    </div>
  </div>
</template>
<style>
 .j2{
   text-align: left;
 }
 .h1{
   text-align: right;
 }

</style>
