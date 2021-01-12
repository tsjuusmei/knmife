<script>
  import Clouds from '../molecules/Clouds.svelte';
</script>

<style>
  * {
    margin: 0;
    padding: 0;
  }

  h1 {
    font-family: 'Sora';
    font-size: 100px;
    font-weight: 700;
    margin: auto;
    z-index: 1000;
    color: var(--darkblue);
  }

  header {
    max-width: none;
    background: url('../images/bg.white.svg') repeat-x bottom;
    background-size: 70%;
    background-color: var(--grey);
    text-align: center;
    height: 100vh;
    display: flex;
    flex-direction: column;
    margin-bottom: -1%;
  }

  img {
    position: relative;
    width: 80px;
    bottom: 4vh;
    margin: 0 auto;
    animation: pulse 2s 3s ease-out infinite;
    z-index: 1000;
  }

  span {
    font-size: 0.4em;
    font-weight: 700;
  }

  @keyframes pulse {
    0% {
      transform: none;
    }
    50% {
      transform: translateY(-0.5rem);
    }
    80% {
      transform: none;
    }
    100% {
      transform: none;
    }
  }
</style>

<header>
  <h1>De invloed van <br /> COVID-19 op de <br />NO<span>2</span> uitstoot</h1>
  <a href="#intro">
    <img src="../images/arrowdown.blue.svg" class="bounce" alt="" />
  </a>
  <Clouds />
</header>
