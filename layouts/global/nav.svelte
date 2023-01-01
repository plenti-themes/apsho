<script>
  export let user;
</script>

<nav class="main-nav navbar navbar-expand-lg headroom headroom--pinned headroom--top">
    <div class="container-fluid">
      <!-- Logo -->
      <a class="navbar-brand" href=".">
        <img class="logo-main" src="assets/logo.png" alt="logo-white">
      </a>
      <!-- Toogle Button -->
      <button class="navbar-toggler collapsed" type="button" data-toggle="collapse" data-target="#mainNav">
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <div class="collapse navbar-collapse nav-list" id="mainNav">
        <!-- Navigation Links -->
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href=".">Home </a>
          </li>
          <li class="nav-item">
            <a class="nav-link scroll-to" href="#about">About </a>
          </li>
          <li class="nav-item">
            <a class="nav-link scroll-to" href="#services">Services </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/blog/">Blog</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="." on:click={$user.login}>login</a>
          </li>
        </ul>
        <div class="account-list list-inline">
          <li class="list-inline-item">
            <a href="/contact/" class="btn btn-sm btn-violate">Get in Touch</a>
          </li>
        </div>
      </div>
    </div>
  </nav>