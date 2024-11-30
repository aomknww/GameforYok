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

        .next-button {
            margin-top: 20px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
            background-color: #4CAF50;
            color: white;
        }

        .next-button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <!-- รูปภาพซองจดหมาย -->
    <div class="envelope">
        <img src="IMG_1219.jpeg" alt="Envelope">
    </div>

    <!-- ปุ่มที่แสดงข้างล่างรูป -->
    <div class="options">
        <button onclick="selectAnswer('รัก')">รัก</button>
        <button onclick="selectAnswer('ไม่รัก')">ไม่รัก</button>
    </div>

    <div class="result" id="result"></div>

    <!-- ปุ่ม "ข้อถัดไป" -->
    <div id="next-button-container" style="display: none;">
        <button class="next-button" onclick="nextStep()">ข้อถัดไป</button>
    </div>

    <script>
        // เมื่อเลือกคำตอบ
        function selectAnswer(answer) {
            document.getElementById('result').textContent = 'คุณเลือก: ' + answer;

            // แสดงปุ่ม "ข้อถัดไป" หลังจากเลือกคำตอบ
            document.getElementById('next-button-container').style.display = 'block';

            // ซ่อนปุ่มเลือกคำตอบ
            document.querySelector('.options').style.display = 'none';
        }

        // เมื่อคลิก "ข้อถัดไป"
        function nextStep() {
            alert("ไปยังขั้นตอนถัดไป!");
            // ที่นี่คุณสามารถใส่โค้ดสำหรับขั้นตอนถัดไป หรือเปลี่ยนหน้าเว็บตามที่ต้องการ
        }
    </script>

</body>
</html>
