# HTML_3
simple mouse event
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mouse Events</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 80px;
            background: #f5f5f5;
        }

        h2 {
            color: #333;
        }

        #box {
            background-color: #4CAF50;
            color: white;
            padding: 15px 30px;
            font-size: 20px;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0,0,0,0.2);
        }

        #box:hover {
            background-color: #45a049;
            transform: scale(1.05);
        }

        #box:active {
            background-color: #3e8e41;
            transform: scale(0.98);
        }
    </style>
</head>
<body>
    <h2>Mouse Events</h2>
    <button id="box">Click Me</button>

    <script>
        let box = document.getElementById("box");

        box.onmouseover = () => box.innerText = "Mouse Over";
        box.onmouseout  = () => box.innerText = "Mouse Out";
        box.onclick     = () => box.innerText = "Mouse Click";
    </script>
</body>
</html>
