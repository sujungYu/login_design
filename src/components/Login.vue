<template>
<div>
    <h1>offco</h1>
    <h2>로그인 유지<input type="checkbox"></h2>
    <input class="form" type="text" placeholder="아이디"><br>
    <input class="form" type="password" placeholder="비밀번호"><br>
    <button class="bt_login_form" v-on:click="login">로그인</button><br>
    <button class="bt_signup_form" v-on:click="signup">회원가입</button>
    
</div>
</template>

<script>
export default {
    data: function() {
        return{

        }
    },
    methods: {
        login() {
            this.$router.replace('home')
        },
        signup() {
            this.$router.replace('signup')
        }
    }

}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kite+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Gothic+A1&display=swap');
body {
    font-size: 10px;
    background-color: rgb(254, 249, 239);
    text-align: center;
}

h1 {
    display: inline-block;
    font-family: 'Kite One', sans-serif;
    font-weight: lighter;
    color: rgb(255, 134, 94);
    font-size: 9em;
    width: 62.5vw;
    height: 22.8vh;
    margin-top: 0.45em;
    margin-bottom: 0;
  }
  h2 {
      margin-left: auto;
      margin-right: 2em;
      font-weight: lighter;
      font-family: 'Gothic A1', sans-serif;
      font-size: 1.3em;
      width: 28.1vw;
      height: 2.63vh;
      margin-top: 2.31em;
  }
  .form {
      display: inline-block;
      width: 82vw;
      height: 6.1vh;
      margin-left: 0;
      margin-bottom: 1.15em;
      border:1px solid rgba(162, 210, 255, 100);
      border-radius: 15px;
  }
  .bt_login_form {
      font-family: 'Gothic A1', sans-serif;
      font-size: 2.6em;
      width: 82vw;
      height: 9vh;
      border: rgb(28, 31, 34);
      border-radius: 15px;
      background-color: rgb(162, 210, 255);

  }
  .bt_signup_form {
      font-family: 'Gothic A1', sans-serif;
      font-size: 2.6em;
      width: 82vw;
      height: 9vh;
      border:1px solid rgb(255, 134, 94);
      border-radius: 15px;
      background-color: white;
    
      
  }
</style>