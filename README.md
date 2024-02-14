# cartoon-canvas-using-html-css

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>cartoon using html</title>
    <style>
        canvas {
            border: 1px solid black;
        }
    </style>
</head>
<body>
    <canvas id="cartoon canvas" width="400" height="400"></canvas>

    <script>
    
        var canvas = document.getElementById("cartoon canvas");
        var ctx = canvas.getContext("2d");

        // Draw Saraswati Mata
        ctx.lineWidth = 2;
        ctx.strokeStyle = "#000"; // black color

        // Head
        ctx.beginPath();
        ctx.arc(200, 100, 50, 0, Math.PI * 2);
        ctx.stroke();

        // Eyes
        ctx.beginPath();
        ctx.arc(180, 85, 5, 0, Math.PI * 2);
        ctx.arc(220, 85, 5, 0, Math.PI * 2);
        ctx.fillStyle = "#000"; // black color
        ctx.fill();

        // Nose
        ctx.beginPath();
        ctx.moveTo(200, 100);
        ctx.lineTo(200, 120);
        ctx.stroke();

        // Mouth
        ctx.beginPath();
        ctx.arc(200, 125, 10, 0, Math.PI, false);
        ctx.stroke();

        // Hair
        ctx.beginPath();
        ctx.moveTo(150, 50);
        ctx.lineTo(250, 50);
        ctx.moveTo(160, 60);
        ctx.lineTo(240, 60);
        ctx.moveTo(170, 70);
        ctx.lineTo(230, 70);
        ctx.stroke();

        // Veena
        ctx.beginPath();
        ctx.moveTo(170, 200);
        ctx.lineTo(230, 200);
        ctx.quadraticCurveTo(250, 210, 230, 220);
        ctx.lineTo(170, 220);
        ctx.quadraticCurveTo(150, 210, 170, 200);
        ctx.stroke();
        ctx.beginPath();
        ctx.moveTo(170, 220);
        ctx.lineTo(150, 240);
        ctx.lineTo(80, 240);
        ctx.lineTo(110, 220);
        ctx.stroke();
        ctx.beginPath();
        ctx.moveTo(230, 220);
        ctx.lineTo(250, 240);
        ctx.lineTo(320, 240);
        ctx.lineTo(290, 220);
        ctx.stroke();

        // Hands
        ctx.beginPath();
        ctx.moveTo(120, 150);
        ctx.lineTo(70, 200);
        ctx.lineTo(70, 280);
        ctx.stroke();
        ctx.beginPath();
        ctx.moveTo(280, 150);
        ctx.lineTo(330, 200);
        ctx.lineTo(330, 280);
        ctx.stroke();

        // Legs
        ctx.beginPath();
        ctx.moveTo(150, 330);
        ctx.lineTo(150, 400);
        ctx.stroke();
        ctx.beginPath();
        ctx.moveTo(250, 330);
        ctx.lineTo(250, 400);
        ctx.stroke();
    </script>
</body>
</html>
