<script>
    export let feature1, feature2;
</script>
<section class="feature" id="about">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6">
          <div class="feature-image">
            <img src="{feature1.image1.image}" class="feature-image-shape1" style="left: -25%; top: 10%;" alt="{feature1.image1.alt}">
            <img src="{feature1.image2.image}" alt="{feature1.image2.alt}">
            <img src="{feature1.image3.image}" style="right: -13%; top: 45%;" class="feature-image-shape2" alt="{feature1.image3.alt}">
          </div>
        </div>
        <div class="col-lg-6">
          <div class="feature-content ml-25">
            <h2>
              {feature1.title}
            </h2>
            <p>
              {feature1.body}
            </p>
            <a href="." data-text="Try It Free" class="btn btn-primary">
              <span>{feature1.link.title}</span>
            </a>
          </div>
        </div>
      </div>
      <div class="row align-items-center">
        <div class="col-lg-6 order-2 order-lg-1">
          <div class="feature-content mr-25">
            <h2>
              {feature2.title}
            </h2>
            <p>
              {feature2.body}
            </p>
            <div class="feature-content-list">
              <ul>
                <li>
                  <i class="ti-check"></i>
                  <p>{feature2.items.item1}</p>
                </li>
                <li>
                  <i class="ti-check"></i>
                  <p>{feature2.items.item2}</p>
                </li>
                <li>
                  <i class="ti-check"></i>
                  <p>{feature2.items.item3}</p>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-lg-6 order-1 order-lg-2">
          <div class="feature-image">
            <img src="{feature2.image1.image}" class="feature-image-shape3" style="right: -25%; top: 10%;" alt="{feature2.image1.alt}">
            <img src="{feature2.image2.image}" alt="{feature2.image2.alt}">
            <img src="{feature2.image3.image}" style="left: -20%; top: 42%;" class="feature-image-shape4" alt="{feature2.image3.alt}">
          </div>
        </div>
      </div>
    </div>
  </section>