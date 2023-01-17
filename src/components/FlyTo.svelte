<script>
  function flyTo() {
    map.flyTo(
      {
        center: [-75.49375, 39.05163],
        zoom: 24,
      },
      { duration: 2000 }
    );
  }
</script>

<button on:click={flyTo} id="flyTo">Recenter</button>
