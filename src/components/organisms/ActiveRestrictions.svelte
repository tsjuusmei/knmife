<script>
  let city = 'madrid';
  function madrid() {
    city = 'madrid';
  }
  function milan() {
    city = 'milan';
  }
  function lyon() {
    city = 'lyon';
  }
  function liverpool() {
    city = 'liverpool';
  }
  let city2 = 'madrid';
  function madrid2() {
    city2 = 'madrid';
  }
  function milan2() {
    city2 = 'milan';
  }
  function lyon2() {
    city2 = 'lyon';
  }
  function liverpool2() {
    city2 = 'liverpool';
  }
</script>

<section>
  <div>
    <div class="container">
      <h2 class="ta-center">
        Vergelijking NO<sub>2</sub> uitstoot tussen steden
      </h2>

      <p class="padding-24">
        Hier onder kan je gemakkelijk de uitstoot tussen twee steden
        vergelijken. De stad kan je boven de grafiek selecteren. In de grafiek
        staan ook balken, die aangeven wanneer welke maatregel actief is. De
        legenda hiervan staat onder de grafiek. De maatregel is te herkennen aan
        het patroon in de balk.
      </p>

      <div class="chart-container">
        <div>
          <div class="buttons">
            <button on:click={madrid}>Madrid</button>
            <button on:click={milan}>Milaan</button>
            <button on:click={lyon}>Lyon</button>
            <button on:click={liverpool}>Liverpool</button>
          </div>
          <div class="group">
            <img
              src="/images/charts/{city}chart.png"
              alt="NO2 data van deze stad"
            />
          </div>
        </div>
        <div>
          <div class="buttons">
            <button on:click={madrid2}>Madrid</button>
            <button on:click={milan2}>Milaan</button>
            <button on:click={lyon2}>Lyon</button>
            <button on:click={liverpool2}>Liverpool</button>
          </div>
          <div class="group">
            <img
              src="/images/charts/{city2}chart.png"
              alt="NO2 data van deze stad"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style type="text/scss">
  section {
    position: relative;
    z-index: 99;
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
      background: hsla(186, 33%, 94%, 1);
    }
  }

  .chart-container {
    display: flex;
    margin: 0 -20rem;
    justify-content: space-evenly;

    & > div {
      width: 50rem;
    }
  }

  .buttons {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    margin-bottom: 4rem;
  }

  button::before {
    content: ' ';
    display: inline-block;
    height: 1.2em;
    width: 1.2em;
    margin-right: 10px;
    border-radius: 4px;
    vertical-align: middle;
  }

  button:nth-child(1) {
    grid-area: 1 / 1 / 2 / 2;
  }
  button:nth-child(2) {
    grid-area: 1 / 2 / 2 / 3;
  }
  button:nth-child(3) {
    grid-area: 1 / 3 / 2 / 4;
  }
  button:nth-child(4) {
    grid-area: 1 / 4 / 2 / 5;
  }

  button:nth-child(1)::before {
    background: var(--madrid);
  }

  button:nth-child(2)::before {
    background: var(--milan);
  }

  button:nth-child(3)::before {
    background: var(--lyon);
  }

  button:nth-child(4)::before {
    background: var(--liverpool);
  }

  button {
    font-size: 1.2em;
    background: transparent;
    box-shadow: 0px 0px 0px transparent;
    border: 2px solid transparent;
    text-shadow: 0px 0px 0px transparent;
    border-radius: 4px;
  }

  button:hover {
    border: 2px solid rgb(97, 97, 97);
  }

  .group {
    width: 100%;
    margin: 0 auto;
  }

  .group img {
    position: relative;
    width: 100%;
  }
</style>
