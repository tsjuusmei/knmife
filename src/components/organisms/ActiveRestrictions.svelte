<script>
  import ChartExample from '../molecules/ChartExample.svelte';
</script>

<style type="text/scss">
  section {
    &::before,
    &::after {
      content: url('../../../images/shape-rounded.svg');
      margin: -4px 0;
      display: block;
    }

    &::after {
      transform: rotate(180deg);
    }

    & > div {
      background: #ededed;
    }
  }
</style>

<section>
  <div>
    <ChartExample />
  </div>
  <!-- <section>
    <div class="container">
      <h3>Actieve maatregelen weergegeven per week</h3>

      <p>
        De maatregelen hieronder hebben het meeste invloed op de uitstoot van NO2.
        Door deze maatregelen is er minder verkeer op de wegen, en dus ook minder
        uitstoot. De uitstoot tijdens deze maatregelen is ook duidelijk een stuk
        minder, zoals hieronder staat aangetoont in een paar kleine
        vergelijkingen.
      </p>

      <h4>Madrid</h4>
      <img src="./images/madridrestrictions.svg" alt="" />

      <h4>Milan</h4>
      <img src="./images/milanrestrictions.svg" alt="" />

      <h4>Lyon</h4>
      <img src="./images/lyonrestrictions.svg" alt="" />

      <h4>Liverpool</h4>
      <img src="./images/liverpoolrestrictions.svg" alt="" />
    </div>
  </section> -->

</section>
