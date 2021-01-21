<script>
  
</script>

<section>
  <div class="container">
    <div class="buttons">
      <p>Madrid</p>
      <p>Milaan</p>
      <p>Lyon</p>
      <p>Liverpool</p>
    </div>
   <div class="group">
      <img src="/images/charts/madridchart.svg" alt="">
    </div>
  </div>
</section>

<style>
  .buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
  }

  p:nth-child(1) { grid-area: 1 / 1 / 2 / 2; }
  p:nth-child(2) { grid-area: 1 / 2 / 2 / 3; }
  p:nth-child(3) { grid-area: 1 / 3 / 2 / 4; }
  p:nth-child(4) { grid-area: 1 / 4 / 2 / 5; }


  .group {
    display: block;
    position: relative;
    width: 100%;
    margin: 0 auto;
  }

  .group img {
    position: absolute;
    width: 100%;
    left: 0;
    top: 0;
    right: 0;
  }
</style>
