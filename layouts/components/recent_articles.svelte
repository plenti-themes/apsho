<script>
    import { sortByDate } from '../scripts/sortByDate.svelte';
    export let title, link, allContent;
</script>
<section class="blog-post" id="blog">
    <div class="container">
      <div class="row">
        <div class="col-lg-10 mx-auto">
          <div class="section-title">
            <h2>{title}</h2>
          </div>
        </div>
      </div>
      <div class="row justify-content-center">
        {#each sortByDate(allContent.filter(content => content.type === "posts")) as post,i}
            {#if i < 3}
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
            {/if}
        {/each}
        <div class="see-all-post col-12">
          <a href="blog" data-text="See all posts" class="btn btn-primary">
            <span>{link.title}</span>
          </a>
        </div>
      </div>
    </div>
  </section>