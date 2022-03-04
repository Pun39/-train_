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
      <h1 class="t">
        กรอกข้อมูลสถานประกอบการ
      </h1><br>

      <v-form
        ref="form"
        v-model="valid"
        lazy-validation
      >
        <h4 class="t1">
          รหัสนักศึกษา
        </h4>

        <v-text-field
          v-model="id"
          :rules=" รหัสนักศึกษา"
          label=" รหัสนักศึกษา"
          required
          outlined
          color="indigo lighten-4"
          light
        />

        <h4 class="t1">
          ที่อยู่
        </h4>

        <v-text-field
          v-model="id_p"
          :rules="ที่อยู่"
          label="ที่อยู่"
          required
          outlined
          light
          color="indigo lighten-4"
        />

        <h4 class="t1">
          ชื่อสถานประกอบการ
        </h4>

        <v-text-field
          v-model="name_o"
          :rules=" ชื่อสถานประกอบการ"
          label=" ชื่อสถานประกอบการ"
          required
          outlined
          light
          color="indigo lighten-4"
        />
        <h4 class="t1">
          ที่อยู่สถานประกอบการ
        </h4>

        <v-text-field
          v-model="id_g"
          :rules=" ที่อยู่สถานประกอบการ "
          label=" ที่อยู่สถานประกอบการ "
          required
          outlined
          light
          color="indigo lighten-4"
        />
        <v-btn href="/detal_t" class="btn  blue accent-2 rounded">
          NEXT
        </v-btn>
      </v-form><br>
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
