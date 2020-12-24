<template>
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md0>
            <div class="d-flex flex-column justify-space-between align-center">
              <v-img
                :lazy-src="require('../assets/KHDT-logo.png')"
                max-height="140"
                max-width="140"
                :src="require('../assets/KHDT-logo.png')"
              ></v-img>
            </div>
            <h1>Hệ thống CMS hiển thị chỉ số báo cáo</h1>
            <br>
            <v-layout align-center justify-center>
            <v-flex xs12 sm8 md4>
              <v-card color="#F3F3F3" flat>
              <v-toolbar dark color="#F3F3F3" flat>
                <v-toolbar-title
                  ><span id="login-title">Đăng nhập</span></v-toolbar-title
                >
                <v-spacer></v-spacer>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-text-field
                    name="login"
                    label="Tên đăng nhập"
                    type="text"
                    outlined
                    dense
                  ></v-text-field>
                  <v-text-field
                    id="password"
                    name="password"
                    label="Mật khẩu"
                    type="password"
                    outlined
                    dense
                  ></v-text-field>
                  <v-spacer></v-spacer>
                  <v-btn color="primary" block>ĐĂNG NHẬP</v-btn>
                </v-form>
              </v-card-text>
            </v-card>
            </v-flex>
            </v-layout>
            <br />
            <span>Bản quyền thuộc Bộ Kế hoạch và Đầu tư</span>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: "Login",
  components: {},
  data: () => ({
    drawer: null,
  }),
  props: {
    source: String,
  },
};
</script>

<style scoped>
#login-title {
  color: black;
}

.v-card--flat{
  box-shadow: none;
}
</style>
