<script>
  import Molecules from '../molecules/Molecules.svelte';
</script>

<style>
  section {
    height: 100vh;
    background-color: white;
    margin-bottom: -2%;
  }

  h2 {
    font-family: 'Sora';
    font-size: 72px;
    text-align: center;
    margin: 5% auto;
    color: var(--darkblue);
  }

  sub {
    font-size: var(--sub);
  }
</style>

<section>
  <Molecules />

  <div class="container">
    <h2>Wat is NO<sub>2</sub>?</h2>

    <p>
      De uitstoot van NO<sub>2</sub>
      is de afgelopen jaren veel te hoog. Door COVID-19 zijn er verschillende
      maatregelen van pas gekomen, waardoor het vervoer en producties
      verminderden. De invloed van deze maatregelen staan in dit artikel
      verwerkt. Stikstofdioxide (NO<sub>2</sub>) is een gas dat in Nederland
      voor een groot gedeelte door het autoverkeer wordt geproduceerd. Het is
      daarom een belangrijke indicator voor de luchtverontreiniging door
      verkeer. Langs grote wegen komen hoge concentraties voor die over een
      afstand van enkele kilometers afnemen tot lage concentraties. Bovendien
      draagt Stikstofdioxide ook bij aan smog.
    </p>
  </div>
</section>
