<script>
  export let user;
  let y, navActive;

const toggleMenu = () => {
  navActive = !navActive;
}

const scroll = e => {
  document.getElementById(e.target.hash.substring(1)).scrollIntoView();
}

</script>
<svelte:window bind:scrollY={y}/>


<nav class="main-nav navbar navbar-expand-lg headroom headroom--pinned headroom--top {y > 50 ? ' active' : ''}">
    <div class="container-fluid">
      <!-- Logo -->
      <a class="navbar-brand" href=".">
        <img class="logo-main" src="logo.png" alt="logo-white">
      </a>
      <!-- Toogle Button -->
      <button class="navbar-toggler collapsed" on:click={toggleMenu} type="button" data-toggle="{navActive ? ' active' : ''}" data-target="#mainNav">
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
        <span class="icon-bar"></span>
      </button>
      <div class="collapse navbar-collapse nav-list {navActive ? ' active' : ''} {y > 20 ? ' sticky' : ''}" on:click={toggleMenu} id="mainNav">
        <!-- Navigation Links -->
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a on:click|preventDefault={e => scroll(e)} class="nav-link" href=".">Home </a>
          </li>
          <li class="nav-item">
            <a on:click|preventDefault={e => scroll(e)} class="nav-link scroll-to" href="#about">About </a>
          </li>
          <li class="nav-item">
            <a on:click|preventDefault={e => scroll(e)} class="nav-link scroll-to" href="#services">Services </a>
          </li>
          <li class="nav-item">
            <a on:click|preventDefault={e => scroll(e)} class="nav-link" href="blog/">Blog</a>
          </li>
          <li class="nav-item">
            <a on:click|preventDefault={e => scroll(e) } on:click={$user.menu} class="nav-link" href=".">login</a>
          </li>
        </ul>
        <div class="account-list list-inline">
          <li class="list-inline-item">
            <a on:click|preventDefault={e => scroll(e)} href="contact/" class="btn btn-sm btn-violate">Get in Touch</a>
          </li>
        </div>
      </div>
    </div>
  </nav>