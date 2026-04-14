<h1>Welcome to ScreenStack</h1>
<script>
  import MovieCard from "$lib/components/MovieCard.svelte";

  let { data } = $props();
  let movies = data.movies;
</script>

<p><i>Daten und Bilder generiert mit ChatGPT und DALL-E</i></p>

<div class="row">
  {#each movies as movie}
    <div class="col-sm-6 col-md-4 col-lg-3 mb-2 gx-2">
      <MovieCard movie={movie}></MovieCard>
    </div>
  {/each}
</div>