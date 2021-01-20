<script>
  import 'chart.js';
  import { onMount } from 'svelte';

  function createChart() {
    var ctx = document.getElementById('myChart').getContext('2d');
    var myChart = new Chart(ctx, {
      type: 'horizontalBar',
      data: {
        datasets: [
          {
            label: 'Bar Dataset',
            data: [10, 30, 50, 50],
            // type: 'horizontalBar'
          },
          {
            label: 'Line Dataset',
            data: [{x: 10, y: 10},
                   {x: 20, y: 10},
                   {x: 30, y: 40},
                   {x: 40, y: 40}],

            // Changes this dataset to become a line
            type: 'line',
          },
        ],
        labels: [10, 20, 30, 40],
      },
      options: {
        scales: {
          yAxes: [
            {
              ticks: {
                beginAtZero: true,
              },
            },
          ],
        },
      },
    });
  }

  onMount(createChart);
</script>

<div class="container">
  <canvas id="myChart" />
</div>
