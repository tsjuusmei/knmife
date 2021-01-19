<script>
  import StayHome from '../molecules/StayHome.svelte';
  import Teleworking from '../molecules/Teleworking.svelte';
  import MassGather from '../molecules/MassGather.svelte';
  import Closepub from '../molecules/Closepub.svelte';
</script>

<style>
  section {
    height:fit-content;
    background-color: #EDEDED;
    /* background: url('../images/rounded.bg.gray.svg') no-repeat;
    background-size: cover;
    background-position: center; */
    padding: 3px 0;
  }

  ul {
    list-style-type: none;
    display: flex;
    margin: 110px;
    justify-content: space-between;
    padding: 0;
  }
</style>

<div class="roundededge">
  <section>
    <div class="container">
      <h3>Welke maatregelen hebben invloed op NO<sub>2</sub></h3>

      <p>
        De onderstaande maatregelen zullen een grote invloed kunnen hebben op NO<sub>2</sub> uitstoot. Door de maatregelen wordt er namelijk veel verkeer op stop gezet, wat de uitstoot erg verminderd aangezien vervoer de grootste uitstoter is van NO<sub>2</sub>.
        
        Deze maatregelen zijn aan de hand van satellietdata via de google earth
        engine uitgekozen en vergeleken met peroides waarin de maatregelen niet actief waren.
      </p>

      <ul>
        <li>
          <StayHome />
        </li>
        <li>
          <Teleworking />
        </li>
        <li>
          <MassGather />
        </li>
        <li>
          <Closepub />
        </li>
      </ul>
    </div>
  </section>
</div>
