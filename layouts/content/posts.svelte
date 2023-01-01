<script>
    export let title, bodyText, subHeading, list, image1, image2, pubDate, author;
</script>
<section class="page-header blog-single-header">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <h2>
            {title}
          </h2>
          <div class="post-meta">
            <ul>
              <li>
                <img src="{author.avatar}" alt="{author.altText}">
              </li>
              <li>
                <h5>
                  {author.name}
                </h5>
              </li>
              <li>
                {pubDate}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="blog-single">
    <div class="container">
      <div class="row">
        <div class="col-lg-10 mx-auto">
          <article class="blog-single-post">
            <p>
              {bodyText}
            </p>
            <p>
                {bodyText}
            </p>
            <img src="{image1.source}" alt="{image1.altText}">
            <p>
              {bodyText}
            </p>
            <h2>{subHeading}</h2>
            <ul>
              <li>{list.item1}</li>
              <li>{list.item2}</li>
              <li>{list.item3}</li>
              <li>{list.item4}</li>
              <li>{list.item5}</li>
            </ul>
            <img src="{image2.source}" alt="{image2.altText}">
            <p>
              {bodyText}<br>
              <br>
              {bodyText}
            </p>
          </article>
        </div>
      </div>
    </div>
  </section>