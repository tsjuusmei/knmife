<script>
  
</script>

<section>
  <div class="container">
    <ul>
      <li>Madrid</li>
      <li>Milaan</li>
      <li>Lyon</li>
      <li>Liverpool</li>
    </ul>
   <div class="group">
      <img src="/images/charts/madridbar.svg" alt="">
      <img src="/images/charts/madridline.svg" alt="">
    </div>
  </div>
</section>

<style>
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

  .group img:nth-child(2) {
    padding-left: 4.5%;
    padding-right: 10%;
    padding-bottom: 5%;
  }
</style>
