<script>
  export let title, env;
</script>

<head>
  <meta charset='utf-8'>
  <meta name='viewport' content='width=device-width,initial-scale=1'>

  <title>{ title }</title>
  <base href="{ env.local ? '/' : env.baseurl }">
  <script type="module" src="/spa/ejected/main.js"></script>
  <link rel="stylesheet" href="/assets/themify-icons/themify-icons.css">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.6.2/dist/css/bootstrap.min.css" integrity="sha384-xOolHFLEh07PJGoPkLv1IbcEPTNtaed2xpHsD9ESMhqIYd0nLMwNLD69Npy4HI+N" crossorigin="anonymous">
  <link href="https://fonts.googleapis.com/css2?family==Poppins:400,500,600,700&display=swap" rel="stylesheet">
  <link rel="icon" type="image/svg+xml" href="/assets/logo.svg">
  <link rel='stylesheet' href='/spa/bundle.css'>
  <link rel='stylesheet' href='assets/global.css'>
</head>
