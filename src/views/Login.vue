<template>
  <form @submit.prevent="login" class="form border">
    <h2 class="form-heading">Login</h2>
    <input
      class="form-input border-input"
      type="email"
      v-model="email"
      placeholder="Email"
    />
    <input
      class="form-input border-input"
      type="password"
      v-model="password"
      placeholder="Password"
    />
    <button type="submit" class="form-btn border">Login</button>
    <div>
      <p>Don't have an account? <router-link to="/register" class="register">Register</router-link></p>
    </div>
  </form>
</template>
<script>
export default {
  data() {
    return {
      email: "",
      password: "",
    };
  },
  methods: {
  login(){
    const subscriber = {
      email: this.email,
      password: this.password,
  }
    fetch('https://capstone-final-backend.herokuapp.com/subscribers', {
     method: 'PATCH',
     body: JSON.stringify(subscriber),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  }
})
  .then((response) => response.json())
  .then((json) => {
   localStorage.setItem("jwt", json.jwt);
   alert("User logged in");
   this.$router.push({ name: "All blogs"});
  })
  .catch((err) => {
    alert(err);
  });
  },
 },
};
</script>
<style>
.border {
border: none !important;
}

input{
    background-color: #e8f0fe;
}
.form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 40px;
  gap: 20px;
  width: 100%;
  margin-inline: auto;
  max-width: 600px;
  margin-top: 150px;
}

.form-heading {
  text-align: center;
  text-transform: uppercase;
}

.form-input,
.form-btn {
  border: none;
  outline: none;
  padding: 20px;
}

.form-btn {
  cursor: pointer;
  transition: all 0.1s linear;
}

.form-btn:hover {
  transform: scale(1.05);
}

.form-social-login {
  display: flex;
  justify-content: space-between;
}

.form-social-btn {
  width: 45%;
  color: #333;
} 
p{
  font-size: 25px;
}
.signup {
  font-size: 25px;
  color: blue;
}
.signup:hover{
  color: blue;
  border-bottom:1px solid blue ;
}
</style>
