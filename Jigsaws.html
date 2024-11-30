<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>เกมจิ๊กซอ</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 50px;
        }

        .puzzle-container {
            display: grid;
            grid-template-columns: repeat(3, 100px);
            grid-gap: 5px;
            justify-content: center;
            margin-top: 20px;
        }

        .puzzle-piece {
            width: 100px;
            height: 100px;
            background-size: cover;
            cursor: pointer;
        }

        .hidden {
            display: none;
        }

        #message {
            font-size: 20px;
            margin-top: 20px;
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

    <h2>ลากชิ้นส่วนจิ๊กซอให้ตรงช่อง</h2>

    <div class="puzzle-container" id="puzzle-container">
        <!-- จิ๊กซอ 9 ชิ้น -->
        <div class="puzzle-piece" id="piece-1" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-2" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-3" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-4" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-5" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-6" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-7" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-8" style="background-image: url('IMG_1219.jpeg');"></div>
        <div class="puzzle-piece" id="piece-9" style="background-image: url('IMG_1219.jpeg');"></div>
    </div>

    <!-- ข้อความเมื่อมีการตรวจสอบ -->
    <div id="message"></div>

    <!-- ปุ่มตกลง -->
    <div id="next-button-container" class="hidden">
        <button class="next-button" onclick="checkPuzzle()">ตกลง</button>
    </div>

    <script>
        let correctPositions = [0, 1, 2, 3, 4, 5, 6, 7, 8]; // ตัวเลขที่บ่งบอกตำแหน่งที่ถูกต้อง
        let currentPositions = []; // ตำแหน่งที่ผู้ใช้ลากไว้
        let draggedPiece = null; // ชิ้นส่วนที่กำลังลาก

        // ให้ความสามารถในการลากและวาง
        document.querySelectorAll('.puzzle-piece').forEach((piece, index) => {
            piece.setAttribute('draggable', 'true');
            piece.addEventListener('dragstart', (e) => {
                draggedPiece = e.target;
            });

            piece.addEventListener('dragover', (e) => {
                e.preventDefault();
            });

            piece.addEventListener('drop', (e) => {
                e.preventDefault();
                if (draggedPiece) {
                    let targetId = e.target.id;
                    let draggedId = draggedPiece.id;
                    // ถ้ามีการวางลงบนช่องเดียวกัน
                    if (draggedId !== targetId) {
                        // สลับตำแหน่งระหว่างชิ้นส่วน
                        let targetIndex = parseInt(targetId.split('-')[1]);
                        let draggedIndex = parseInt(draggedId.split('-')[1]);

                        currentPositions[draggedIndex] = targetIndex;
                        currentPositions[targetIndex] = draggedIndex;

                        // เปลี่ยนตำแหน่งของชิ้นส่วน
                        let targetStyle = e.target.style.backgroundImage;
                        e.target.style.backgroundImage = draggedPiece.style.backgroundImage;
                        draggedPiece.style.backgroundImage = targetStyle;
                    }
                }
            });
        });

        // เมื่อผู้ใช้เริ่มเล่นเกม
        function startPuzzle() {
            currentPositions = Array.from({ length: 9 }, (_, i) => i);
            document.getElementById('next-button-container').classList.remove('hidden');
        }

        // ฟังก์ชันตรวจสอบว่าเกมจิ๊กซอถูกต้องหรือไม่
        function checkPuzzle() {
            if (JSON.stringify(currentPositions) === JSON.stringify(correctPositions)) {
                document.getElementById('message').textContent = "ถูกต้อง!";
                setTimeout(() => {
                    alert("ไปยังขั้นตอนถัดไป!");
                    // สามารถใส่การเปลี่ยนหน้าเว็บที่นี่ เช่น `window.location.href = "nextPage.html";`
                }, 1000);
            } else {
                document.getElementById('message').textContent = "ผิด! ลองใหม่อีกครั้ง";
            }
        }

        // เริ่มเกมเมื่อโหลดหน้า
        window.onload = startPuzzle;
    </script>

</body>
</html>
