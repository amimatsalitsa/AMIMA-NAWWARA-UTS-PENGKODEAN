<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amima Nawwara | UTS Pengkodean</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            overflow-x: hidden;
        }

        .container {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 24px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            max-width: 800px;
            width: 100%;
            padding: 50px 40px;
            text-align: center;
            animation: fadeInUp 0.8s ease-out;
            position: relative;
            overflow: hidden;
        }

        .container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(118, 75, 162, 0.1), transparent);
            animation: shine 3s infinite;
        }

        @keyframes shine {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea, #764ba2);
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 25px;
            font-size: 50px;
            color: white;
            font-weight: 700;
            box-shadow: 0 10px 30px rgba(118, 75, 162, 0.4);
            animation: pulse 2s infinite;
            position: relative;
            z-index: 1;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        h1 {
            font-size: 2.2em;
            color: #2d3748;
            margin-bottom: 10px;
            font-weight: 700;
            position: relative;
            z-index: 1;
        }

        .subtitle {
            color: #764ba2;
            font-size: 1.1em;
            font-weight: 600;
            margin-bottom: 30px;
            position: relative;
            z-index: 1;
        }

        .divider {
            width: 60px;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            border-radius: 2px;
            margin: 0 auto 30px;
            position: relative;
            z-index: 1;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 35px;
            position: relative;
            z-index: 1;
        }

        .info-card {
            background: linear-gradient(135deg, #f7fafc, #edf2f7);
            border-radius: 16px;
            padding: 25px 15px;
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }

        .info-card:hover {
            transform: translateY(-5px);
            border-color: #764ba2;
            box-shadow: 0 10px 25px rgba(118, 75, 162, 0.2);
        }

        .info-card .icon {
            font-size: 2em;
            margin-bottom: 10px;
        }

        .info-card h3 {
            color: #4a5568;
            font-size: 0.85em;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        .info-card p {
            color: #2d3748;
            font-weight: 600;
            font-size: 1em;
        }

        .description {
            color: #718096;
            line-height: 1.8;
            margin-bottom: 35px;
            font-size: 0.95em;
            position: relative;
            z-index: 1;
            padding: 0 10px;
        }

        .btn {
            display: inline-block;
            padding: 14px 40px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1em;
            transition: all 0.3s ease;
            box-shadow: 0 8px 20px rgba(118, 75, 162, 0.4);
            position: relative;
            z-index: 1;
            letter-spacing: 0.5px;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 30px rgba(118, 75, 162, 0.6);
        }

        .btn:active {
            transform: translateY(-1px);
        }

        footer {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #e2e8f0;
            color: #a0aec0;
            font-size: 0.85em;
            position: relative;
            z-index: 1;
        }

        /* Responsif untuk HP */
        @media (max-width: 600px) {
            .container {
                padding: 35px 25px;
            }

            h1 {
                font-size: 1.6em;
            }

            .subtitle {
                font-size: 0.95em;
            }

            .avatar {
                width: 90px;
                height: 90px;
                font-size: 38px;
            }

            .info-grid {
                grid-template-columns: 1fr;
            }

            .btn {
                padding: 12px 30px;
                font-size: 0.9em;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Avatar -->
        <div class="avatar">AN</div>

        <!-- Nama -->
        <h1>Amima Nawwara</h1>
        <p class="subtitle">UTS Mata Kuliah Pengkodean</p>

        <div class="divider"></div>

        <!-- Info Cards -->
        <div class="info-grid">
            <div class="info-card">
                <div class="icon">📚</div>
                <h3>Mata Kuliah</h3>
                <p>Pengkodean</p>
            </div>
            <div class="info-card">
                <div class="icon">📝</div>
                <h3>Jenis Tugas</h3>
                <p>Ujian Tengah Semester</p>
            </div>
            <div class="info-card">
                <div class="icon">💻</div>
                <h3>Teknologi</h3>
                <p>HTML & CSS</p>
            </div>
        </div>

        <!-- Deskripsi -->
        <p class="description">
            Halaman ini merupakan hasil implementasi kode untuk memenuhi tugas 
            <strong>Ujian Tengah Semester (UTS)</strong> pada mata kuliah 
            <strong>Pengkodean</strong>. Dibuat dengan desain modern, responsif, 
            dan interaktif menggunakan HTML dan CSS.
        </p>

        <!-- Tombol -->
        <a href="https://github.com/amimatsalitsa" target="_blank" class="btn">
            🚀 Kunjungi GitHub Saya
        </a>

        <!-- Footer -->
        <footer>
            <p>© 2026 Amima Nawwara — Dibuat dengan ❤️ untuk UTS Pengkodean</p>
        </footer>
    </div>
</body>
</html>
