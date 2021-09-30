<template>
  <v-container>
    <v-text-field
      v-model="name"
      label="お名前"
      outlined
      required
    ></v-text-field>
    <v-text-field
      v-model="mail"
      label="メールアドレス"
      outlined
      required
    ></v-text-field>
    <v-text-field
      v-model="form"
      label="お問い合わせ内容"
      required
      outlined
      height="200"
    ></v-text-field>
    <v-container class="text-center"
      ><v-btn class="ma-1" style="width:120px" to="/">キャンセル</v-btn
      ><v-btn class="ma-1" color="primary" style="width:120px"
        >送信</v-btn
      ></v-container
    >
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      name: "",
      mail: ""
    };
  },
  created() {
    var userAgent = window.navigator.userAgent.toLowerCase();
    console.log(userAgent);
  }
};
</script>

<style></style>
