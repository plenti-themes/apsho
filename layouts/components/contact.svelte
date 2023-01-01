<script>
    export let terms, form, button;
</script>
<section class="contact">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 mx-auto">
          <form class="contact-form row" method="POST" action="{form.url}">
            <div class="col-lg-6">
              <input type="text" class="form-control" placeholder="{form.name}" name="name" required="">
            </div>
            <div class="col-lg-6">
              <input type="email" class="form-control" placeholder="{form.email}" name="email" required="">
            </div>
            <div class="col-12">
              <input type="text" class="form-control" placeholder="{form.subject}">
            </div>
            <div class="col-12">
              <textarea class="form-control" placeholder="{form.message}" required="" cols="30" rows="7"></textarea>
            </div>
            <div class="col-6 align-self-center">
              <div class="form-check">
                <input class="form-check-input" type="checkbox" id="termCondition">
                <label class="form-check-label" for="termCondition">
                  {terms.text1}<a href="{terms.url}">{terms.text2}</a>
                </label>
              </div>
            </div>
            <div class="col-6 text-right">
              <button class="btn btn-primary-filled" type="submit" formtarget="_blank">
                {button.text}
              </button>
            </div>
          </form>
<!--           <p class="contact-form-generator mt-3">
            <strong>** </strong> <a href="https://fabform.io/" target="_blank">Static website forms</a>
          </p> -->
        </div>
      </div>
    </div>
  </section>