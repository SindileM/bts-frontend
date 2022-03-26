<template>
  <header id="header" class="header d-flex align-items-center fixed-top">
    <div class="container-fluid container-xl d-flex align-items-center justify-content-between">

      <a href="index.html" class="logo d-flex align-items-center">
        <!-- Uncomment the line below if you also wish to use an image logo -->
        <!-- <img src="assets/img/logo.png" alt=""> -->
        <h1>ZenBlog</h1>
      </a>

      <nav id="navbar" class="navbar">
        <ul>
          <li><a href="Allblogs.vue">Allblogs</a></li>
          <li><a href="single-post.html">Single Post</a></li>
          <li class="dropdown"><a href="category.html"><span>Categories</span> <i class="bi bi-chevron-down dropdown-indicator"></i></a>
            <ul>
              <li><a href="search-result.html">Search Result</a></li>
              <li><a href="#">Drop Down 1</a></li>
              <li class="dropdown"><a href="#"><span>Deep Drop Down</span> <i class="bi bi-chevron-down dropdown-indicator"></i></a>
                <ul>
                  <li><a href="#">Deep Drop Down 1</a></li>
                  <li><a href="#">Deep Drop Down 2</a></li>
                  <li><a href="#">Deep Drop Down 3</a></li>
                  <li><a href="#">Deep Drop Down 4</a></li>
                  <li><a href="#">Deep Drop Down 5</a></li>
                </ul>
              </li>
              <li><a href="#">Drop Down 2</a></li>
              <li><a href="#">Drop Down 3</a></li>
              <li><a href="#">Drop Down 4</a></li>
            </ul>
          </li>

          <li><a href="about.html">About</a></li>
          <li><a href="contact.html">Contact</a></li>
        </ul>
      </nav><!-- .navbar -->

      <div class="position-relative">
        <a href="#" class="mx-2"><span class="bi-facebook"></span></a>
        <a href="#" class="mx-2"><span class="bi-twitter"></span></a>
        <a href="#" class="mx-2"><span class="bi-instagram"></span></a>

        <a href="#" class="mx-2 js-search-open"><span class="bi-search"></span></a>
        <i class="bi bi-list mobile-nav-toggle"></i>

        <!-- ======= Search Form ======= -->
        <div class="search-form-wrap js-search-form-wrap">
          <form action="search-result.html" class="search-form">
            <span class="icon bi-search"></span>
            <input type="text" placeholder="Search" class="form-control">
            <button class="btn js-search-close"><span class="bi-x"></span></button>
          </form>
        </div><!-- End Search Form -->

      </div>

    </div>

  </header>
</template>

<script>

</script>

<style>
.header {
  height: 90px;
  transition: all 0.5s;
  z-index: 997;
  background: #f2f2f2;
}
.header.sticked {
  height: 70px;
}
.header .logo img {
  max-height: 40px;
  margin-right: 6px;
}
.header .logo h1 {
  font-size: 30px;
  font-weight: 700;
  color: var(--color-default);
  font-family: var(--font-primary);
}

.search-form-wrap {
  position: absolute;
  right: 0;
  top: 0;
  z-index: 9;
  transition: 0.3s all ease;
  visibility: hidden;
  opacity: 0;
}
.search-form-wrap .search-form {
  position: relative;
}
.search-form-wrap .search-form .form-control {
  width: 300px;
  border: none;
  box-shadow: 0 15px 20px -10px rgba(var(--color-black-rgb), 0.1);
  padding-left: 40px;
  padding-right: 40px;
}
.search-form-wrap .search-form .form-control:active, .search-form-wrap .search-form .form-control:focus {
  outline: none;
  box-shadow: none;
}
.search-form-wrap .search-form .icon {
  position: absolute;
  left: 0;
  top: 7px;
  opacity: 0.5;
  left: 10px;
}
.search-form-wrap .search-form .btn {
  position: absolute;
  top: 2px;
  right: 4px;
  padding: 0;
  margin: 0;
  line-height: 1;
  font-size: 30px;
}
.search-form-wrap .search-form .btn:active, .search-form-wrap .search-form .btn:focus {
  outline: none;
  box-shadow: none;
}
.search-form-wrap.active {
  visibility: visible;
  opacity: 1;
}

section {
  scroll-margin-top: 70px;
}

</style>