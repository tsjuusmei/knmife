<script>
  import StayHome from '../molecules/StayHome.svelte'
  import Teleworking from '../molecules/Teleworking.svelte'
  import MassGather from '../molecules/MassGather.svelte'
  import Closepub from '../molecules/Closepub.svelte'
</script>

<style>
  p {
    width: 35%;
  }

  section {
    height: 100vh;
    background: url("../images/rounded.bg.gray.svg") no-repeat;
    background-size: 100%;
    padding: 0 150px;
  }

  h3 {
    font-family: "Sora";
    color: var(--darkblue);
    font-size: 30px;
    padding-top: 5%;
    text-align: center;
  }

  p {
    width: 55%;
    line-height: 2em;
    margin: auto;
  }

  ul {
    list-style-type: none;
    display: flex;
    margin: 110px;
    justify-content: space-between;
    padding: 0;
  }
</style>

<section>
  <div class="container">
    <h3>Welke maatregelen hebben wij gekozen en waarom</h3>

    <p>
      We hebben de onderstaande maatregelen gekozen om te gebruiken voor ons
      onderzoek. Deze keuzes hebben wij aan de hand van een bestand dat alle
      actieve maatregelen per land weergeeft in een schema en de google earth
      engine gemaakt.
    </p>

    <ul>
      <li><StayHome /></li>
      <li><Teleworking /></li>
      <li><MassGather /></li>
      <li><Closepub /></li>
    </ul>
  </div>
</section>
