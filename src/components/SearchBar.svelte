<script>
  import maplibre from "maplibre-gl";

  let addressSearch;

  function searchLocation() {
    // get the value of the search input bar
    const searchInput = document.querySelector("input").value;

    console.log(searchInput);
  }
</script>

<div>
  <!-- create a search input bar for searching addresses -->
  <input bind:value={addressSearch} type="search" name="geoloc" id="" />
  <button on:click={searchLocation}>Search</button>
</div>

<!-- <script>
  let geocoder;
  let results = [];
  let query = "";
  let maptiler;

  onMount(async () => {
    //create a new instance of the geocoder
    geocoder = await new maptiler.Geocoder({
      key: "pMcJ43PmWeoAuyjWcvbN", // replace with your own API key
    });
  });

  async function search(query) {
    // use the geocoder to search for the query
    results = await geocoder.search({ query });
  }
</script>

<input
  type="text"
  bind:value={query}
  placeholder="Enter an address or place name"
/>
<button on:click={() => search(query)}>Search</button>

{#if results.length > 0}
  <ul>
    {#each results as result}
      <li>
        {result.formatted} ({result.position.lat}, {result.position.lng})
      </li>
    {/each}
  </ul>
{/if} -->
<style>
  div {
    position: absolute;
    z-index: 1;
    background: none;
    padding: 10px;
    margin-top: 15px;
    margin-left: 5%;
    border-radius: 4px;
    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
  }
</style>
