<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Color and Number Prediction</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        h1 {
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <h1>Color and Number Prediction</h1>
    <button onclick="predict()">Predict</button>
    <p id="prediction"></p>

    <script>
        function predict() {
            var colors = ['Red', 'Green'];
            var color = colors[Math.floor(Math.random() * colors.length)];
            var number = Math.floor(Math.random() * 10); // Generate a random number between 0 and 9
            var size = number >= 5 ? "big" : "small"; // Determine if the number is big or small

            // Display prediction
            var predictionText = "Color: " + color + ", Number: " + number + ", " + size;
            document.getElementById("prediction").textContent = predictionText;
        }
    </script>
</body>
</html>

