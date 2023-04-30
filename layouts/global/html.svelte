<script>
  import Head from './head.svelte';
  import Nav from './nav.svelte';
  import Footer from './footer.svelte'
  import Login from './login.svelte';
  export let content, layout, allContent, allLayouts, env, user;

  let hash;
  onMount(async () => {
    hash = window.location.hash;
  });
</script>

<html lang="en">
  <Head title={content.filename}  {env} {...content.fields}  />
  <body data-aos-easing="ease" data-aos-duration="400" data-aos-delay="0">
    {#if user && $user.isAuthenticated}
    <svelte:component this={$user.menu} {user} bind:content={content} />
    {/if}
    <Login bind:hash {user} />
    <Nav />
    <svelte:component this={layout} {...content.fields} {allContent} {allLayouts} {content} />
    <Footer />
  </body>
</html>

<!-- <style>
  :global(nav) ~ main header {
    top: 41px;
  }
</style> -->