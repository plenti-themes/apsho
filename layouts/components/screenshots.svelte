<script>
  export let title,
    description,
    sliderFrame,
    image1,
    image2,
    image3,
    image4,
    image5;
  const screenshots = [
    {
      id: "slick-slide01",
      scr: "{image1.src}",
      alt: "{image1.alt}",
    },
    {
      id: "slick-slide02",
      scr: "{image2.src}",
      alt: "{image2.alt}",
    },
    {
      id: "slick-slide03",
      scr: "{image3.src}",
      alt: "{image3.alt}",
    },
    {
      id: "slick-slide04",
      scr: "{image4.src}",
      alt: "{image4.alt}",
    },
    {
      id: "slick-slide05",
      scr: "{image5.src}",
      alt: "{image5.alt}",
    },
    {
      id: "slick-slide06",
      scr: "{image1.src}",
      alt: "{image1.alt}",
    },
  ];
</script>

<section class="screenshots">
  <div class="container">
    <div class="row">
      <div class="col-lg-8 mx-auto">
        <div class="screenshots-title">
          <h2>
            {title}
          </h2>
          <p>
            {description}
          </p>
        </div>
      </div>
    </div>
  </div>
  <div class="screenshots-wrapper">
    <div class="screenshots-slider-frame">
      <img src={sliderFrame.src} alt={sliderFrame.alt} />
    </div>
    <div class="screenshots-slider slick-initialized slick-slider slick-dotted">
      <div class="slick-list draggable" style="padding: 0px;">
        <div
          class="slick-track"
          style="opacity: 1; width: 4410px; transform: translate3d(-1715px, 0px, 0px);"
        >
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-6"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image1.src} alt={image1.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-5"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-4"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image3.src} alt={image3.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-3"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image4.src} alt={image4.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-2"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image5.src} alt={image5.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="-1"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide"
            data-slick-index="0"
            aria-hidden="true"
            tabindex="-1"
            role="tabpanel"
            id="slick-slide00"
            aria-describedby="slick-slide-control00"
            style="width: 245px;"
          >
            <img src={image1.src} alt={image1.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-active"
            data-slick-index="1"
            aria-hidden="false"
            tabindex="-1"
            role="tabpanel"
            id="slick-slide01"
            aria-describedby="slick-slide-control01"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-active"
            data-slick-index="2"
            aria-hidden="false"
            tabindex="-1"
            role="tabpanel"
            id="slick-slide02"
            aria-describedby="slick-slide-control02"
            style="width: 245px;"
          >
            <img src={image3.src} alt={image3.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-current slick-active slick-center"
            data-slick-index="3"
            aria-hidden="false"
            tabindex="0"
            role="tabpanel"
            id="slick-slide03"
            aria-describedby="slick-slide-control03"
            style="width: 245px;"
          >
            <img src={image4.src} alt={image4.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-active"
            data-slick-index="4"
            aria-hidden="false"
            tabindex="0"
            role="tabpanel"
            id="slick-slide04"
            aria-describedby="slick-slide-control04"
            style="width: 245px;"
          >
            <img src={image5.src} alt={image5.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-active"
            data-slick-index="5"
            aria-hidden="false"
            tabindex="0"
            role="tabpanel"
            id="slick-slide05"
            aria-describedby="slick-slide-control05"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="6"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image1.src} alt={image1.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="7"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="8"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image3.src} alt={image3.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="9"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image4.src} alt={image4.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="10"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image5.src} alt={image5.alt} />
          </div>
          <div
            class="screenshots-slider-item slick-slide slick-cloned"
            data-slick-index="11"
            aria-hidden="true"
            tabindex="-1"
            style="width: 245px;"
          >
            <img src={image2.src} alt={image2.alt} />
          </div>
        </div>
      </div>

      <ul class="slick-dots" style="" role="tablist">
        <li class="" role="presentation">
          <button
            type="button"
            role="tab"
            id="slick-slide-control00"
            aria-controls="slick-slide00"
            aria-label="1 of 2"
            tabindex="-1">1</button
          >
        </li>
        <li role="presentation" class="">
          <button
            type="button"
            role="tab"
            id="slick-slide-control01"
            aria-controls="slick-slide01"
            aria-label="2 of 2"
            tabindex="-1">2</button
          >
        </li>
        <li role="presentation" class="">
          <button
            type="button"
            role="tab"
            id="slick-slide-control02"
            aria-controls="slick-slide02"
            aria-label="3 of 2"
            tabindex="-1">3</button
          >
        </li>
        <li role="presentation" class="slick-active">
          <button
            type="button"
            role="tab"
            id="slick-slide-control03"
            aria-controls="slick-slide03"
            aria-label="4 of 2"
            tabindex="0"
            aria-selected="true">4</button
          >
        </li>
        <li role="presentation">
          <button
            type="button"
            role="tab"
            id="slick-slide-control04"
            aria-controls="slick-slide04"
            aria-label="5 of 2"
            tabindex="-1">5</button
          >
        </li>
        <li role="presentation">
          <button
            type="button"
            role="tab"
            id="slick-slide-control05"
            aria-controls="slick-slide05"
            aria-label="6 of 2"
            tabindex="-1">6</button
          >
        </li>
      </ul>
    </div>
  </div>
</section>
