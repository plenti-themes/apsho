<script>
    export let title, subtitle, email;
</script>
<section class="page-header">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <h2>{title}</h2>
          <p>
            {subtitle}
            <a href="{email.url}">{email.text}</a>
          </p>
        </div>
      </div>
    </div>
  </section>