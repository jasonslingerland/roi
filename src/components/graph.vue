

<script>

import { Bar, Line } from 'vue-chartjs'

export default {

    extends: Line,
    mounted () {
      // Overwriting base render method with actual data.
      this.renderChart({
        labels: ['0', '1', '2', '3', '4', '5'],
        datasets: [
          {
            label: 'Onshape',
            backgroundColor: '#3d5afe',
            data: [20, 40, 60, 80, 100, 120]
          },
          {
            label: 'Solidworks',
            backgroundColor: '#f87979',
            data: [60, 120, 180, 240, 300, 360]
          }

        ]
      })
    }



}
</script>

<style>
</style>
