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
    <div class="l  white">
      <v-sheet
        class="h"
        color="indigo darken-4"
        elevation="1"
        height="50"
        outlined
        rounded
        width="330"
      >
        <h1>
          ข้อมูลนักเรียนนักศึกษา
        </h1><br>
      </v-sheet><br>
      <div class="lo">
        <v-row>
          <v-col md="5">
            <img src="@/assets/img/1.png" width="80%">
          </v-col>
          <v-col md="6">
            <br><br>
            <h3 class="t">
              นางสาวเทคนิค ชัยภูมิ
            </h3>
          </v-col>
        </v-row><br>
        <v-sheet
          class="h"
          color="indigo darken-4"
          elevation="1"
          height="10"
          outlined
          width="327"
        />
        <div class="t">
          <h3 class="h1">
            ข้อมูล <br>
            <br>รหัสนักศึกษา:633090100xx <br>
            <br>เลขที่บัตรประชาชน:136960000xxxx<br>
            <br>ระดับชั้น ปวส.2 ห้อง E5<br>
            <br> แผนกเทคโนโลยีสารสนเทศ<br>
            <br>ครูที่ปรึกษา : นายxxx xxx<br>
            <br>ที่อยู่ : 111 ม.10 ต.ในเมือง อ.เมือง จ.ชัยภูมิ 36000<br>
            <br>เบอร์โทรติดต่อ : 062174xxxx<br>
            <br>ชื่อบิดา : นายxxxx xxx<br>
            <br>ชื่อมารดา : นางxxxx xxx<br><br>
          </h3>
        </div>
      </div>

      <v-btn href="/ad_std" class="btn  blue accent-2 rounded">
        NEXT
      </v-btn><br>
    </div>
  </div>
</template>
<style>
  .h1{
    text-align: left;
  }
  .h2{
    text-align: right;

  }
  .t{
    color: black;
  }
.t1{
    color: black;
    text-align: left;
  }
</style>
