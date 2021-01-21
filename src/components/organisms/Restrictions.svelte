<script>
  import StayHome from '../molecules/StayHome.svelte';
  import Teleworking from '../molecules/Teleworking.svelte';
  import MassGather from '../molecules/MassGather.svelte';
  import Closepub from '../molecules/Closepub.svelte';
</script>

<style type="text/scss">
  section {
    position: relative;
    z-index: 99;
    margin-top: -6%;
    padding: 0;

    &::before,
    &::after {
      content: url('/images/shape-rounded.svg');
      margin: -5px 0;
      display: block;
    }

    &::after {
      transform: rotate(180deg);
    }

    & > div {
      padding: 4rem 0;
      background: hsla(186, 33%, 94%, 1)
    }
  }

  ul {
    display: flex;
    justify-content: space-between;
    list-style: none;
  }
</style>

<section>
  <div>
    <div class="container">
      <h2 class="ta-center">Welke maatregelen hebben invloed op NO<sub>2</sub></h2>

      <p class="padding-24">
        De onderstaande maatregelen zullen een grote invloed kunnen hebben op NO<sub
          >2</sub
        >
        uitstoot. Door de maatregelen wordt er namelijk veel verkeer op stop
        gezet, wat de uitstoot erg verminderd aangezien vervoer de grootste
        uitstoter is van NO<sub>2</sub>. Deze maatregelen zijn aan de hand van
        satellietdata via de google earth engine uitgekozen en vergeleken met
        peroides waarin de maatregelen niet actief waren.
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
  </div>
</section>
