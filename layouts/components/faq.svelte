<script>
    export let title, description, accordion1, accordion2, accordion3;
</script>
<section class="faq" id="faq">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6">
          <div class="faq-content">
            <h2>
              {title}
            </h2>
            <p>
              {description}
            </p>
          </div>
        </div>
        <div class="col-lg-6">
          <div class="faq-accordion" id="faqAccordion">
            <div class="faq-accordion-item">
              <div class="header">
                <h5 class="mb-0">
                  <button class="btn btn-link collapsed" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="false">
                    {accordion1.title}
                  </button>
                </h5>
              </div>
  
              <div id="collapseOne" class="collapse" data-parent="#faqAccordion" style="">
                <div class="body">
                 {accordion1.description}
                </div>
              </div>
            </div>
            <div class="faq-accordion-item">
              <div class="header">
                <h5 class="mb-0">
                  <button class="btn btn-link collapsed" type="button" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false">
                    {accordion2.title}
                  </button>
                </h5>
              </div>
              <div id="collapseTwo" class="collapse" data-parent="#faqAccordion">
                <div class="body">
                  {accordion2.description}
                </div>
              </div>
            </div>
            <div class="faq-accordion-item">
              <div class="header" id="headingThree">
                <h5 class="mb-0">
                  <button class="btn btn-link collapsed" type="button" data-toggle="collapse" data-target="#collapseThree">
                    {accordion3.title}
                  </button>
                </h5>
              </div>
              <div id="collapseThree" class="collapse" data-parent="#faqAccordion">
                <div class="body">
                  {accordion3.description}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>