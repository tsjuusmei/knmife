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

  #maatregelen {
    height: 100vh;
    background-image: url("../images/rounded.bg.gray.svg");
    background-size: cover;
    padding: 0 150px;
  }

  h3 {
    font-family: "Sora";
    color: #00255a;
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
    margin: 150px;
    justify-content: space-between;
  }
</style>

<div id="maatregelen">
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
