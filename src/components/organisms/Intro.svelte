<script>
  import Molecules from '../molecules/Molecules.svelte';
</script>

<style type="text/scss">
  section {
    position: relative;
    overflow: hidden;
    padding-bottom: 18rem;
    background: url('../../../public/images/juniperphoton-KKFKrOu3BVc-unsplash.jpg') no-repeat center;
    background-size: cover;

    & > div {
      position: relative;
      z-index: 99;

      h2,
      p {
        color: #fff;
      }

      &:first-child {
        position: absolute;

      }
    }

    &::after {
      content: '';
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      z-index: 1;
      background-color: rgba( #1f3b62, .6);
    }
  }

  h2 {
    text-align: center;
  }

</style>

<section>
  <Molecules />

  <div class="container">
    <h2 class="ta-center padding-02">Wat is NO<sub>2</sub>?</h2>

    <p class="padding-20">
      Stikstofdioxide (NO<sub
        >2</sub
      >) is een gas dat in Nederland voor een groot gedeelte door het
      autoverkeer wordt geproduceerd. Het is daarom een belangrijke indicator
      voor de luchtverontreiniging door verkeer. Langs grote wegen komen hoge
      concentraties voor die over een afstand van enkele kilometers afnemen tot
      lage concentraties. Bovendien draagt Stikstofdioxide ook bij aan smog.
    </p>
  </div>
</section>
