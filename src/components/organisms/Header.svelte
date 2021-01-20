<script>
  import Clouds from '../molecules/Clouds.svelte';
</script>

<style type="text/scss">
  header {
    position: relative;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: url('../images/bg.white.svg') repeat-x bottom;
    background-size: 70%;

    &::after {
      content: '';
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      z-index: -999;
      background: linear-gradient(90deg, hsla(186, 33%, 94%, 1) 0%, hsla(216, 41%, 79%, 1) 100%);;
    }
  }

  img {
    position: absolute;
    width: 80px;
    bottom: 4vh;
    margin: 0 auto;
    animation: pulse 2s 3s ease-out infinite;
    z-index: 1000;
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
  <h1>Hoe COVID-19 de<br />lucht schoner maakt</h1>
  <img src="../images/arrowdown.blue.svg" class="bounce" alt="" />
  <Clouds />
</header>
