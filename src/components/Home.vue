<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

  </div>
    <!-- <div class="container">
    <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://i.postimg.cc/ZKCcLkxN/teen-driver.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>WELCOME TO URBAN ROOTS</h5>
        <p>
       This platform transforms the university application experience of young South Africans from being complicated and stressful.Urban Roots is a platform that connects students fresh out of high school to various opportunities including – Full-time study, Part-time study, Driving lessons and opportunities.
        This platform transforms the university application experience of young South Africans from being complicated and costly to one which is accessible and less expensive.</p>
      <div class="slider-btn">
        <button>
       <router-link to="/register" class="register">REGISTER</router-link>
      </button>
        <button>
        <router-link to="/login" class="register">LOGIN</router-link>
     </button>
      </div>
      </div>
    </div>
    <div class="carousel-item">
      <img src="https://i.postimg.cc/R09pdsFz/home-slider.jpg" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block">
        <h5>WELCOME TO URBAN ROOTS</h5>
        <p>
       This platform transforms the university application experience of young South Africans from being complicated and stressful.Urban Roots is a platform that connects students fresh out of high school to various opportunities including – Full-time study, Part-time study, Driving lessons and opportunities.
        This platform transforms the university application experience of young South Africans from being complicated and costly to one which is accessible and less expensive.</p>
      <div class="slider-btn">
        <button>
       <router-link to="/register" class="register">REGISTER</router-link>
      </button>
        <button>
        <router-link to="/login" class="register">LOGIN</router-link>
     </button>
      </div>
      </div>
    </div>
    <div class="carousel-item">
      <img src="https://i.postimg.cc/sfQXswjz/blog.png" class="d-block w-100" alt="...">
      <div class="carousel-caption d-none d-md-block"> 
        <h5>WELCOME TO URBAN ROOTS</h5>
        <p>
       This platform transforms the university application experience of young South Africans from being complicated and stressful.Urban Roots is a platform that connects students fresh out of high school to various opportunities including – Full-time study, Part-time study, Driving lessons and opportunities.
        This platform transforms the university application experience of young South Africans from being complicated and costly to one which is accessible and less expensive.</p>
      <div class="slider-btn">
        <button>
       <router-link to="/register" class="register">REGISTER</router-link>
      </button>
        <button>
        <router-link to="/login" class="register">LOGIN</router-link>
     </button>
      </div>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
 </div> -->
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.carousel-item {
  width: 100%;
}
.container {
  padding: 0;
  max-width: 100%;
}
.carousel-inner img {
  width: 100vw ;
  height: 92.5vh;
  object-fit: cover;
}
.carousel-item::before{
  content: "";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background: #000;
  opacity: 0.7;
}
a{
  background-color: red;
  color: white;
  border-radius: 50px;
  padding: 1.5rem 2rem;
  font-size: 1rem;
  text-decoration: none;
  
}
button{
  background: none;
  border: none;
}
.carousel-caption h5{
  font-size: 70px;
  font-weight: 300;
}
.carousel-caption p{
  font-size: 18px;
}

</style>