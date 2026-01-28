<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>My Beautiful Website</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Font Google -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: #f6f8ff;
            color: #333;
        }

        /* ===== HEADER ===== */
        header {
            height: 100vh;
            background: linear-gradient(to right, #667eea, #764ba2);
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            text-align: center;
        }

        header h1 {
            font-size: 60px;
            animation: fadeDown 1.5s ease;
        }

        header p {
            font-size: 22px;
            margin-top: 20px;
            animation: fadeUp 2s ease;
        }

        @keyframes fadeDown {
            from {opacity: 0; transform: translateY(-50px);}
            to {opacity: 1; transform: translateY(0);}
        }

        @keyframes fadeUp {
            from {opacity: 0; transform: translateY(50px);}
            to {opacity: 1; transform: translateY(0);}
        }

        /* ===== SECTION ===== */
        section {
            padding: 80px 10%;
        }

        .title {
            text-align: center;
            font-size: 40px;
            margin-bottom: 40px;
            color: #5a4fcf;
        }

        /* ===== IMAGE ===== */
        .images {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .images img {
            width: 100%;
            border-radius: 20px;
            transition: 0.5s;
            box-shadow: 0 15px 25px rgba(0,0,0,0.2);
        }

        .images img:hover {
            transform: scale(1.05);
        }

        /* ===== VIDEO ===== */
        .video-box {
            display: flex;
            justify-content: center;
        }

        video {
            width: 80%;
            border-radius: 20px;
            box-shadow: 0 15px 30px rgba(0,0,0,0.3);
        }

        /* ===== FOOTER ===== */
        footer {
            background: #5a4fcf;
            color: white;
            text-align: center;
            padding: 30px;
            font-size: 18px;
        }
    </style>
</head>

<body>

    <!-- HEADER -->
    <header>
        <h1>Welcome to My Website</h1>
        <p>Một trang web nhỏ xinh nhưng đầy cảm xúc 💖</p>
    </header>

    <!-- IMAGE SECTION -->
    <section>
        <h2 class="title">📸 Hình ảnh nổi bật</h2>
        <div class="images">
            <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee">
            <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e">
            <img src="https://images.unsplash.com/photo-1496307042754-b4aa456c4a2d">
        </div>
    </section>

    <!-- VIDEO SECTION -->
    <section>
        <h2 class="title">🎬 Video truyền cảm hứng</h2>
        <div class="video-box">
            <video controls>
                <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
                Trình duyệt của bạn không hỗ trợ video.
            </video>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        © 2026 | Designed with ❤️ by Thanh Trúc
    </footer>

</body>
</html>
