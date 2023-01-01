<script>
    export let title, bodyText, allContent;
    let posts = allContent.filter(content => content.type === "posts");
</script>
<section class="page-header">
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-lg-8">
        <h1>{title}</h1>
        <p>
          {bodyText}
        </p>
      </div>
    </div>
  </div>
</section>
<section class="blog">
  <div class="container">
    <div class="row">
    {#each posts as post}
      <div class="col-lg-4 col-md-6">
        <article class="blog-post-item" style="height: 378.328px;">
          <div class="blog-post-thumb">
            <a href="{post.path}">
              <img src="{post.fields.thumbImage.source}" alt="{post.fields.thumbImage.altText}"></a>
          </div>
          <div class="blog-post-content">
            <h2>
              <a href="{post.path}">{post.fields.title}</a>
            </h2>
            <div class="post-author">
              <div class="thumb">
                <img src="{post.fields.author.avatar}" alt="{post.fields.author.altText}">
              </div>
              <div class="meta">
                <h3>{post.fields.author.name}</h3>
                <p>{post.fields.pubDate}</p>
              </div>
            </div>
          </div>
        </article>
      </div>
      {/each}
      <div class="col-lg-12">
        <div class="blog-pagination">
          <nav class="nav-bg">
            <ul class="pagination">
              <li class="page-item active" aria-current="page">
                <span class="page-link">
                  1
                  <span class="sr-only">(current)</span>
                </span>
              </li>
              <li class="page-item"><a class="page-link" href=".">2</a></li>
              <li class="page-item"><a class="page-link" href=".">3</a></li>
              <li class="page-item">
                <a class="page-link" href=".">
                  <i class="ti-angle-right"></i>
                </a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </div>
</section>