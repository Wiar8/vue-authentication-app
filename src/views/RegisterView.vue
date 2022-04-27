<template>
  <div class="register">
    <h2>Register</h2>
    <form>
      <div class="register__input">
        <input type="email" required />
        <label>Email</label>
      </div>
      <div class="register__input">
        <input type="password" required />
        <label>Password</label>
      </div>

      <button class="register__submit" type="submit">Register</button>
    </form>
  </div>
</template>

<style>
.register {
  margin: 100px auto;
  width: 400px;
  padding: 40px;
  background: #282828;
  box-sizing: border-box;
  box-shadow: 0 15px 25px rgba(0, 0, 0, 0.6);
  border-radius: 10px;
}

.register h2 {
  margin-bottom: 30px;
  color: #fff;
  text-align: center;
}

.register .register__input {
  position: relative;
}

.register .register__input input {
  font-size: 18px;
  width: 100%;
  padding: 10px 0;
  color: #fff;
  margin-bottom: 30px;
  border: none;
  border-bottom: 1px solid #fff;
  outline: none;
  background: transparent;
}
.register .register__input label {
  position: absolute;
  top: 0;
  left: 0;
  padding: 10px 0;
  color: #fff;
  pointer-events: none;
  transition: 0.5s;
}

.register .register__input input:focus ~ label,
.register .register__input input:valid ~ label {
  top: -20px;
  left: 0;
  color: #03e9f4;
  font-size: 12px;
}

.register__submit {
  color: #1b1c1b;
  padding: 0.7em 1.7em;
  font-size: 18px;
  border-radius: 0.5em;
  background: #e8e8e8;
  border: none;
  cursor: pointer;
}
</style>
