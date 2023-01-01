<script>
  import Head from './head.svelte';
  import Nav from './nav.svelte';
  import Footer from './footer.svelte'
  export let content, layout, allContent, allLayouts, env, user, adminMenu;
</script>

<html lang="en">
  <Head title={content.filename}  {env} />
  <body data-aos-easing="ease" data-aos-duration="400" data-aos-delay="0">
    {#if user && $user.isAuthenticated}
    <svelte:component this={adminMenu} {user} bind:content={content} />
    {/if}
    <Nav {user} />
    <svelte:component this={layout} {...content.fields} {allContent} {allLayouts} {content} />
    <Footer />
  </body>
</html>

<!-- <style>
  :global(nav) ~ main header {
    top: 41px;
  }
</style> -->