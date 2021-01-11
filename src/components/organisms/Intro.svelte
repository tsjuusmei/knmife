<script>
  import Clouds from "../molecules/Clouds.svelte";
  import Molecules from "../molecules/Molecules.svelte";
</script>

<style>
  #intro {
    height: 100vh;
    background-image: linear-gradient(#e3e3e3, #cccccc);
  }

  h2 {
    font-size: 72px;
    text-align: center;
  }

  p {
    font-size: 16px;
    width: 35%;
    margin-left: 150px;
    line-height: 2em;
  }

  .right {
    margin-left: 50vw;
  }
</style>

<div id="intro">
  <Clouds />
  <Molecules />

  <h2>Wat is NO₂?</h2>

  <p>
    De uitstoot van NO₂ is de afgelopen jaren veel te hoog. Door COVID-19 zijn
    er verschillende maatregelen van pas gekomen, waardoor het vervoer en
    producties verminderden. De invloed van deze maatregelen staan in dit
    artikel verwerkt.
  </p>

  <p class="right">
    Stikstofdioxide (NO₂) is een gas dat in Nederland voor een groot gedeelte
    door het autoverkeer wordt geproduceerd. Het is daarom een belangrijke
    indicator voor de luchtverontreiniging door verkeer. Langs grote wegen komen
    hoge concentraties voor die over een afstand van enkele kilometers afnemen
    tot lage concentraties. Stikstofdioxide draagt bijvoorbeeld bij aan smog.
  </p>
</div>
