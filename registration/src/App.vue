<script setup lang="ts">
</script>

<template>
  <div class="wrap">
    <form action="" method="" class="form">
      <div class="form_title">
        <h2 class="title_text">Регистрация</h2>
      </div>
      <div class="form_item">
        <label for="firsName">Имя</label>
        <input type="text" name="firsName" id="firsName" placeholder="Введите ваше имя" required />
      </div>
      <div class="form_item">
        <label for="lastName">Фамилия</label>
        <input type="text" name="lastName" id="lastName" placeholder="Введите вашу фамилию" required />
      </div>
      <div class="form_item">
        <label for="phone">Номер телефона</label>
        <input type="tel" name="phone" id="phone" placeholder="Введите номер телефона" required />
      </div>
      <div class="form_item">
        <label for="email">Aдрес электронной почты</label>
        <input type="email" name="email" id="email" placeholder="Введите адрес эл. почты" required />
      </div>
      <div class="form_item">
        <label for="password">Пароль </label>
        <input type="password" name="password" id="password" placeholder="Создайте пароль" required />
      </div>
      <div class="form_item">
        <label for="password">Повторите пароль</label>
        <input type="password" name="password" id="repeat-password" placeholder="Повторите пароль" required />
      </div>
      <div class="form_item">
        <input type="submit" id="btn-submit" value="Продолжить" />
      </div>
    </form>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box
}

body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(113, 112, 111);
}

.wrap {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  border: 2px solid #c2c2c2;
  border-radius: 5px;
  width: 50vw;
  height: 85vh;
  background-color: beige;
}

.form_title {
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.title_text {
  font-size: 40px;
  font-weight: 600;
  text-align: center;
  margin: 20px 0;
}

.form_item {
  display: flex;
  flex-direction: column;
  margin-top: 5px;
}

.form_item label {
  font-size: 16px;
  color: #111111;
  margin-bottom: 5px;
}

.form_item label:hover {
  cursor: pointer;
}

.form_item input {
  border: 2px solid #626161;
  border-radius: 5px;
  padding: 5px;
}

.form_item input:focus {
  border: 5px solid #fa4e4e;
  outline: none;
}

.form_item input::placeholder {
  color: #626161;
}

#btn-submit {
  min-width: 60px;
  min-height: 40px;
  background-color: #fa4e4e;
  color: #ffffff;
  border: none;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10px;
  cursor: pointer;
}

#btn-submit:focus,
#btn-submit:hover {
  background-color: #a70606;
}
</style>