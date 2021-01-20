<script>
  import 'chart.js';
  import { onMount } from 'svelte';

  function createChart() {
    var ctx = document.getElementById('myChart').getContext('2d');
    var myChart = new Chart(ctx, {
      type: 'bar',
      data: {
        datasets: [
          {
            label: 'Bar Dataset',
            data: [10, 20, 30, 40],
          },
          {
            label: 'Line Dataset',
            data: [50, 50, 50, 50],

            // Changes this dataset to become a line
            type: 'line',
          },
        ],
        labels: ['January', 'February', 'March', 'April'],
      },
      options: {
        indexAxis: 'y',
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
