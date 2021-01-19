<style>

  section {
    margin-bottom: 10%;
  }

  .list {
    list-style-type: none;
    display: flex;
    justify-content: space-evenly;
    padding: 0;
  }

  .list div {
      display: inline-flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: relative;
      width: 225px;
  }
  
  h5 {
      font-size: 20px;
      color: var(--darkblue);
  }

  .map {
      width: 100%;
      height: 225px;
      position: relative;
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
    font-size: var(--sub)
  }

  .year {
    margin: 10px auto;
    text-align: center;
  }
</style>

<section>
  <div class="container">
    <h3>NO<sub>2</sub> waardes in vergelijking met vorig jaar</h3>
    <p>Hierbij wordt de uitstoot vergeleken ten oopzichte van 2019. Deze afbeeldingen zijn afkomstig uit de Tropomi sateliet, en laten de NO2 uitstoot over een bepaalde periode zien. De data is verzameld over de periode met de meeste NO2 reductie, en vergeleken met dezelfde periode in 2019. <br>De steden staan in het midden van de afbeeldingen.</p>
    <div class="list">
        <div>
            <h5>Madrid</h5>
            <div class="map">
              <img src="../images/no2maps/madrid.2019.jpg" alt="Madrid 2019">
            </div>
            <p class="year">2019</p>
            <p class="year">2020</p>
            <div class="map">
              <img src="../images/no2maps/madrid.2020.jpg" alt="Madrid 2020">
            </div>
        </div>
        <div>
            <h5>Milaan</h5>
            <div class="map">
              <img src="../images/no2maps/milan.2019.jpg" alt="Milaan 2019">
            </div>
            <p class="year">2019</p>
            <p class="year">2020</p>
            <div class="map">
              <img src="../images/no2maps/milan.2020.jpg" alt="Milaan 2020">
            </div>
        </div>
        <div>
            <h5>Lyon</h5>
            <div class="map">
              <img src="../images/no2maps/lyon.2019.jpg" alt="Lyon 2019">
            </div>
            <p class="year">2019</p>
            <p class="year">2020</p>
            <div class="map">
              <img src="../images/no2maps/lyon.2020.jpg" alt="Lyon 2020">
            </div>
        </div>
        <div>
            <h5>Liverpool</h5>
            <div class="map">
              <img src="../images/no2maps/liverpool.2019.jpg" alt="Liverpool 2019">
            </div>
            <p class="year">2019</p>
            <p class="year">2020</p>
            <div class="map">
              <img src="../images/no2maps/liverpool.2020.jpg" alt="Liverpool 2020">
            </div>
        </div>
    </div>
  </div>
</section>
