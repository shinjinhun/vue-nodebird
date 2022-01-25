<template>
  <v-container>
    <v-card>
      <v-form ref="form" v-model="valid" @submit.prevent="onSubmitForm">
        <v-container>
          <v-text-field
                  v-model="email"
                  :rules="emailRules"
                  label="이메일"
                  type="email"
                  required
          />
          <v-text-field
                  v-model="password"
                  :rules="passwordRules"
                  label="비밀번호"
                  type="password"
                  required
          />
          <v-btn color="green" type="submit" :disabled="!valid">로그인</v-btn>
          <v-btn nuxt to="/signup">회원가입</v-btn>
        </v-container>
      </v-form>
    </v-card>
  </v-container>
</template>

<script>

</script>

<style>

</style>
