<style type="text/scss">
  section {
    margin-bottom: 10%;
  }

  .list {
    list-style-type: none;
    display: flex;
    justify-content: space-evenly;
    padding: 0;

    & > div {
      display: inline-flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: relative;
      width: 225px;

      .map:nth-of-type(2) {
        padding-top: 2rem;
      }
    }
  }

  h4 {
    font-size: var(--heading-3);

    &.city {
      display: flex;
      align-items: center;
      position: relative;
      left: 15px;

      &::before {
        content: "";
        left: -10px;
        width: 20px;
        height: 20px;
        border-radius: 50%;
        display: block;
        position: absolute;
        transform: translateX(-100%);
      }

      &-madrid::before {
        background: var(--madrid);
      }

      &-milan::before {
        background: var(--milan);
      }

      &-lyon::before {
        background: var(--lyon);
      }

      &-liverpool::before {
        background: var(--liverpool);
      }
    }
  }

  .map {
    width: 100%;
    height: 225px;
    position: relative;
    padding-bottom: 1rem;

    &:last-child {
      padding-top: 2rem;
    }
  }

  img {
    display: block;
    margin: 0 auto;
    height: 100%;
    width: 100%;
    border-radius: 20px;
    object-fit: cover;
  }

  sub {
    font-size: var(--sub);
  }

  .year {
    font-size: 16px;
    text-align: center;
  }

  .alttext {
    text-align: center;
  }

</style>

<section class="padding-06">
  <div class="container">
    <h2 class="ta-center">NO<sub>2</sub> waardes in vergelijking met vorig jaar</h2>
    <p class="padding-24">
      Als we de uitstoot waardes van 2020 en 2019 vergelijken zijn er erg grote
      verschillen te zien. Deze afbeeldingen zijn afkomstig uit de Tropomi
      sateliet, en geven visueel de NO<sub>2</sub> uitstoot over een bepaalde
      periode zien. De data is verzameld over de periode met de meeste NO<sub
        >2</sub
      > reductie, en vergeleken met dezelfde periode in 2019. De maatregelen met
      betrekking op vervoer hebben dus grote invloed gehad op de uitstoot.
    </p>

    <div class="list">
      <div>
        <h4 class="city city-madrid">Madrid</h4>
        <div class="map">
          <img src="../images/no2maps/madrid.2019.jpg" alt="Madrid 2019" />
        </div>
        <p class="year">2019</p>
        <div class="map">
          <img src="../images/no2maps/madrid.2020.jpg" alt="Madrid 2020" />
        </div>
        <p class="year">2020</p>
      </div>
      <div>
        <h4 class="city city-milan">Milaan</h4>
        <div class="map">
          <img src="../images/no2maps/milan.2019.jpg" alt="Milaan 2019" />
        </div>
        <p class="year">2019</p>
        <div class="map">
          <img src="../images/no2maps/milan.2020.jpg" alt="Milaan 2020" />
        </div>
        <p class="year">2020</p>
      </div>
      <div>
        <h4 class="city city-lyon">Lyon</h4>
        <div class="map">
          <img src="../images/no2maps/lyon.2019.jpg" alt="Lyon 2019" />
        </div>
        <p class="year">2019</p>
        <div class="map">
          <img src="../images/no2maps/lyon.2020.jpg" alt="Lyon 2020" />
        </div>
        <p class="year">2020</p>
      </div>
      <div>
        <h4 class="city city-liverpool">Liverpool</h4>
        <div class="map">
          <img
            src="../images/no2maps/liverpool.2019.jpg"
            alt="Liverpool 2019"
          />
        </div>
        <p class="year">2019</p>
        <div class="map">
          <img
          src="../images/no2maps/liverpool.2020.jpg"
          alt="Liverpool 2020"
          />
        </div>
        <p class="year">2020</p>
      </div>
    </div>

    <p class="alttext padding-20">De steden staan in het midden van de afbeeldingen.</p>
  </div>
</section>
