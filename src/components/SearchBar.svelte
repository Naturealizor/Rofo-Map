<script>
  import maplibre from "maplibre-gl";

  let addressSearch;
  // var geocoder = new maplibre.Geocoder({
  //   accessToken: maplibre.accessToken,
  //   maplibregl: maplibre,
  // });

  function searchLocation() {
    // get the value of the search input bar
    const searchInput = document.querySelector("input").value;

    console.log(addressSearch);
  }
</script>

<div>
  <!-- create a search input bar for searching addresses -->
  <input bind:value={addressSearch} type="search" name="geoloc" id="" />
  <button on:click={searchLocation}>Search</button>
</div>

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
