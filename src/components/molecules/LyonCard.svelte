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
    padding-top: 2rem;
    color: #fff;
    font-size: var(--heading-3);
  }

  h5 {
    margin-top: 0;
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
  }

  img {
    height: 15px;
    padding-right: 4px;
  }

  p {
    font-size: 12px;
    position: absolute;
    display: flex;
    top: 175px;
    align-items: center;
    justify-content: left;
    margin-left: 20px;
  }
</style>

<li>
  <h4>Lyon</h4>
  <div>
    <h5>1.705.000 <br /> <span>Aantal inwoners</span></h5>
    <p><img src="./images/person.lyon.svg" alt="" /> = 100.000</p>
    <PersonRowLightblue />
  </div>
</li>
