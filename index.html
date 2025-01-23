<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Slope Graph</title>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    body { font-family: Arial, sans-serif; margin: 20px; text-align: center; }
    .container { max-width: 800px; margin: auto; }
    input, button { padding: 10px; margin: 10px 5px; }
    #graph-container { width: 100%; height: 400px; margin-top: 20px; }
    .result { margin-top: 20px; }
  </style>
</head>
<body>
  <div class="container">
    <h1>Slope Graph</h1>
    <p>Enter slope equations in the form <code>y = mx + b</code>:</p>
    <div>
      <input type="text" id="equation1" placeholder="e.g., y = 2x + 3">
      <input type="text" id="equation2" placeholder="e.g., y = 2x - 4">
      <button onclick="plotGraph()">Plot Graph</button>
    </div>
    <div id="graph-container">
      <canvas id="slopeGraph"></canvas>
    </div>
    <div class="result" id="result"></div>
  </div>

  <script>
    const ctx = document.getElementById('slopeGraph').getContext('2d');
    let chart;

    function parseEquation(equation) {
      // Extract m and b from the equation "y = mx + b"
      const match = equation.match(/y\s*=\s*([+-]?\d*\.?\d*)x\s*([+-]?\s*\d*\.?\d*)?/i);
      if (!match) return null;

      const m = parseFloat(match[1]) || 0; // Slope (m)
      const b = parseFloat(match[2]?.replace(/\s+/g, '') || 0); // Intercept (b)
      return { m, b };
    }

    function generateLineData(m, b, xRange = [-10, 10]) {
      const data = [];
      for (let x = xRange[0]; x <= xRange[1]; x++) {
        data.push({ x, y: m * x + b });
      }
      return data;
    }

    function plotGraph() {
      const equation1 = document.getElementById('equation1').value.trim();
      const equation2 = document.getElementById('equation2').value.trim();
      const resultDiv = document.getElementById('result');

      // Parse equations
      const line1 = parseEquation(equation1);
      const line2 = parseEquation(equation2);

      if (!line1 || !line2) {
        resultDiv.innerHTML = '<p style="color: red;">Invalid equations. Please use the format "y = mx + b".</p>';
        return;
      }

      // Generate data for lines
      const data1 = generateLineData(line1.m, line1.b);
      const data2 = generateLineData(line2.m, line2.b);

      // Determine if lines are parallel
      const areParallel = line1.m === line2.m;
      resultDiv.innerHTML = areParallel
        ? '<p style="color: green;">The lines are parallel.</p>'
        : '<p style="color: blue;">The lines are not parallel.</p>';

      // Plot graph
      if (chart) chart.destroy(); // Destroy previous chart
      chart = new Chart(ctx, {
        type: 'scatter',
        data: {
          datasets: [
            {
              label: `Line 1: ${equation1}`,
              data: data1,
              borderColor: 'red',
              showLine: true,
            },
            {
              label: `Line 2: ${equation2}`,
              data: data2,
              borderColor: 'blue',
              showLine: true,
            },
          ],
        },
        options: {
          scales: {
            x: { type: 'linear', position: 'bottom', title: { display: true, text: 'X' } },
            y: { title: { display: true, text: 'Y' } },
          },
        },
      });
    }
  </script>
</body>
</html>
