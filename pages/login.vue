<template>
  <div>
    <div class="text-center">
      <v-dialog
        v-model="dialog"
        width="500"
      >
        <v-card>
          <v-card-title class="text-h5 grey lighten-2">
            Status Login
          </v-card-title>

          <v-card-text>
            SUCCESS  LOGIN
          </v-card-text>

          <v-divider />

          <v-card-actions>
            <v-spacer />
            <v-btn
              color="primary"
              text
              @click="dialog = false"
            >
              I accept
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </div>
    <div class="text-center">
      <v-dialog
        v-model="dialog_false"
        width="500"
      >
        <v-card>
          <v-card-title class="text-h5 grey lighten-2">
            Status Login
          </v-card-title>

          <v-card-text>
            ERROR  LOGIN
          </v-card-text>

          <v-divider />

          <v-card-actions>
            <v-spacer />
            <v-btn
              color="primary"
              text
              @click="dialog_false = false"
            >
              I accept
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-dialog>
    </div>
    <div class="g1 indigo lighten-5">
      <br>
      <img src="@/assets/img/user.png" width="90%"><br><br>
    </div><br><br>
    <div class="g2">
      PLEASE ENTER YOUR GMAIL
      <v-text-field
        v-model="email"
        :rules="กรุณาป้อนEmail"
        label="EMAIL"
        required
        filled
        plain
        raised
        rounded
      />
      PLEASE ENTER YOUR PASSWORD
      <v-text-field
        v-model="pass"
        :rules="กรุณากรอกpassword"
        label="PASSWORD"
        required
        filled
        plain
        raised
        rounded
      /> <br>
      <v-btn class="t rounded " light @click="onSave">
        LOGIN
      </v-btn><br><br>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    email: '',
    pass: '',
    dialog: false,
    dialog_false: false
  }),
  methods: {
    async onSave () {
      console.log('Login')
      const res = await fetch('http://localhost:7000/list?email=' +
      this.email + '&pass=' + this.pass)
      const data = await res.json()
      if (data.status > 0) {
        console.log('Login OK')
        this.dialog = true
        setInterval(() => {
          this.dialog = false
          this.$router.push('/user')
        }, 2000)
      } else {
        console.log('Login Error')
        this.dialog_false = true
        setInterval(() => {
          this.dialog_false = false
          // this.$router.push('/login')
        }, 3000)
      }
    }
  }
}
</script>
