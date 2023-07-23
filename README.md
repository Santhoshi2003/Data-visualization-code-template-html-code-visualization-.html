# Data-visualization-code-template-html-code-visualization-.html
visualization.html
<!DOCTYPE html>
<html>
<head>
    <title>Dynamic Data Visualization</title>
    <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
</head>
<body>
    <h1>Data Visualization</h1>
    <div id="plot"></div>

    <script>
        var graphJSON = {{ graphJSON | safe }};

        Plotly.newPlot('plot', graphJSON.data, graphJSON.layout);
    </script>
</body>
</html>
