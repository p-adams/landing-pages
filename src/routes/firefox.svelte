<script context="module" lang="ts">
  export const prerender = true;
</script>

<script lang="ts">
  import Tile from "$lib/Tile.svelte";
  import FirefoxImg from "../assets/firefox/firefox.png";
</script>

<main>
  <section>
    <div class="logo-and-name">
      <img src={FirefoxImg} alt="firefox logo" />
      <div>Firefox</div>
    </div>
    <div class="search-bar">
      <input />
    </div>
    <Tile />
  </section>
</main>

<style>
  main {
    width: 510px;
    margin: 0 auto;
  }
  section {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .logo-and-name {
    display: flex;
    align-items: center;
    margin-bottom: 45px;
  }
  .logo-and-name img {
    width: 82px;
    height: 82px;
  }
  .logo-and-name div {
    display: inline-block;
    font-size: 42px;
    font-weight: 600;
    margin-left: 12px;
  }
  .search-bar {
    width: 100%;
  }
  .search-bar input {
    width: 100%;
    height: 35px;
  }
</style>
