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
      border-radius: 20px;
      background: url('../images/map.placeholder.jpg') no-repeat;
      background-size: cover;
      background-position: center;
  }

  sub {
    font-size: var(--sub)
  }
</style>

<section>
  <div class="container">
    <h3>NO<sub>2</sub> waardes in vergelijking met vorig jaar</h3>
    <div class="list">
        <div>
            <h5>Madrid</h5>
            <div class="map">
            </div>
            <p>2019</p>
            <p>2020</p>
            <div class="map">
            </div>
        </div>
        <div>
            <h5>Milaan</h5>
            <div class="map">
            </div>
            <p>2019</p>
            <p>2020</p>
            <div class="map">
            </div>
        </div>
        <div>
            <h5>Lyon</h5>
            <div class="map">
            </div>
            <p>2019</p>
            <p>2020</p>
            <div class="map">
            </div>
        </div>
        <div>
            <h5>Liverpool</h5>
            <div class="map">
            </div>
            <p>2019</p>
            <p>2020</p>
            <div class="map">
            </div>
        </div>
    </div>
  </div>
</section>
