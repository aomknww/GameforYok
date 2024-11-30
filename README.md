# GameforYok
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>เลือกคำตอบ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 50px;
        }

        .envelope {
            width: 100px;
            height: 100px;
            background-color: #f0e1c1;
            border-radius: 15px;
            margin: 0 auto;
            position: relative;
            cursor: pointer;
        }

        .envelope:before {
            content: "✉";
            font-size: 50px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }

        .options {
            margin-top: 20px;
        }

        .options button {
            padding: 10px 20px;
            margin: 10px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }

        .options button:hover {
            background-color: #ccc;
        }

        .result {
            margin-top: 20px;
            font-size: 18px;
        }
    </style>
</head>
<body>

    <div class="envelope" onclick="openEnvelope()"></div>

    <div class="options" id="options" style="display: none;">
        <button onclick="selectAnswer('รัก')">รัก</button>
        <button onclick="selectAnswer('ไม่รัก')">ไม่รัก</button>
    </div>

    <div class="result" id="result"></div>

    <script>
        function openEnvelope() {
            document.getElementById('options').style.display = 'block';
        }

        function selectAnswer(answer) {
            document.getElementById('result').textContent = 'คุณเลือก: ' + answer;
        }
    </script>

</body>
</html>
