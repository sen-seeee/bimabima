<html lang="zh-CN">
<head>
    <meta charset="UTF-8" />
    <title>毕马毕马原谅我</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
            background-color: #f0f0f0;
        }

        h1 {
            color: #333;
        }

        p {
            font-size: 18px;
            color: #666;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

    <h1>马年摸马有福气！</h1>
    <p id="demo">点击按钮，摸摸毕马？</p>
    <button onclick="changeText()">点击我</button>

    <script>
        const initialText = "点击按钮，摸摸毕马？";
        const messages = [
            "恭喜你摸到了马眼",
            "恭喜你摸到了马头",
            "你摸到了马腿",
            "你摸到了马屁",
            "你什么也没有摸到，要再摸一次吗？",
            "很倒霉，你并不想摸马粪"
        ];

        function changeText() {
            const demo = document.getElementById("demo");
            if (demo.innerHTML === initialText) {
                const randomIndex = Math.floor(Math.random() * messages.length);
                demo.innerHTML = messages[randomIndex];
            } else {
                demo.innerHTML = initialText;
            }
        }
    </script>

</body>
</html>
