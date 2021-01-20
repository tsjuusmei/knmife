<style>
    h3 {
        padding-top: 0;
    }

    div.card {
        border-radius: 20px;
        box-shadow: var(--cardshadow);
        width: auto;
        height: auto;
        padding: 2em 0;
        margin-top: 4em;
    }

    .card > img {
        display:flex;
        margin: 30px 5vw;
    }

    .legend {
        margin: 0 12vw;
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(2, 1fr);
        grid-column-gap: 0px;
        grid-row-gap: 0px;
    }

    p::before {
        content: " ";
        display: inline-block;
        height: 1.2em;
        width: 1.2em;
        margin-right: 10px;
        border-radius: 2px;
        vertical-align: middle;
    }

    p:nth-child(1) { grid-area: 1 / 1 / 2 / 2; }
    p:nth-child(1)::before {
        background: var(--madrid);
    }
    p:nth-child(2) { grid-area: 1 / 2 / 2 / 3; }
    p:nth-child(2)::before {
        background: var(--milan);
    }
    p:nth-child(3) { grid-area: 2 / 1 / 3 / 2; }
    p:nth-child(3)::before {
        background: var(--lyon);
    }
    p:nth-child(4) { grid-area: 2 / 2 / 3 / 3; }
    p:nth-child(4)::before {
        background: var(--liverpool);
    }
    p:nth-child(5) { grid-area: 1 / 3 / 3 / 4; }
    p:nth-child(5)::before {
        border-bottom: 2px dotted red;
        width: 50px;
        height: 5px;
    }
</style>

<div class="card">
    <h3>Gemeten NO<sub>2</sub> waardes tijdens COVID-19</h3>
    <img src="../images/no2graph.svg" alt="barchart">
    <div class="legend">
        <p>Madrid</p>
        <p>Milaan</p>
        <p>Lyon</p>
        <p>Liverpool</p>
        <p>Gemiddelde waarde over periode</p>
    </div>
</div>