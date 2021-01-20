<script>
  import PersonRowLightblue from '../atoms/PersonLightblue.svelte';
</script>

<style>
  div {
    background-color: white;
    width: 225px;
    height: 225px;
    border-radius: 20px;
    margin: auto;
  }

  h4 {
    color: white;
    font-size: 30px;
    text-transform: uppercase;
  }

  h5 {
    font-size: 20px;
    text-align: left;
    line-height: 1em;
    margin-left: 20px;
    padding-top: 25px;
  }

  h5 span {
    font-size: 16px;
    color: #a5a5a5;
    font-weight: 300;
  }

  li {
    position: relative;
    width: 275px;
    height: 375px;
    background-color: var(--lyon);
    border-radius: 20px;
    text-align: center;
    /* box-shadow: var(--cardshadow) */
  }

  img {
    height: 15px;
  }

  p {
    font-size: 12px;
    position: absolute;
    display: flex;
    top: 175px;
    align-items: center;
    justify-content: left;
    margin-left: 20px;
    margin-top: 15px;
  }
</style>

<li>
  <h4>Lyon</h4>
  <div>
    <h5>1.705.000 <br /> <span>Aantal inwoners</span></h5>
    <p><img src="./images/person.lyon.svg" alt="" /> =100.000</p>
    <PersonRowLightblue />
  </div>
</li>
