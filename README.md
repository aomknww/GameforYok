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
            margin: 0 auto;
            position: relative;
            cursor: pointer;
        }

        .envelope img {
            width: 100%;
            height: 100%;
            object-fit: cover;
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

    <!-- ใช้รูปภาพแทนไอคอนซองจดหมาย -->
    <div class="envelope" onclick="openEnvelope()">
        <img src="IMG_1219.jpeg" alt="Envelope">
    </div>

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
