<script>
  import PersonRowLightred from '../atoms/PersonRowLightred.svelte';
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
    padding: 10% 10% 8%;
    line-height: 1em;
    margin-bottom: 0;
  }

  h5 span {
    font-size: 16px;
    color: #a5a5a5;
    font-weight: 300;
  }

  li {
    width: 275px;
    height: 375px;
    background-color: var(--lightred);
    border-radius: 20px;
    text-align: center;
  }
</style>

<li>
  <h4>Madrid</h4>
  <div>
    <h5>6.559.000 <br /> <span>Aantal inwoners</span></h5>
    <PersonRowLightred />
  </div>
</li>
