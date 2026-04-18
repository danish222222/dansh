<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - Muhammad Danish Athallah Sutandy</title>
    <style>
        /* CSS Reset & Dasar */
        * { box-sizing: border-box; } /* Tambahan biar responsif di dalam iframe */
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #f4f7f6;
            color: #333;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
        }
        
        /* Desain Card Portfolio */
        .card {
            background: #ffffff;
            width: 100%;
            max-width: 600px;
            border-radius: 12px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            overflow: hidden;
            text-align: center;
            padding: 40px 20px;
            margin-top: 20px;
            border-top: 5px solid #007bff;
        }

        .profile-img {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid #f4f7f6;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            margin-bottom: 15px;
            transition: transform 0.3s;
        }
        
        .profile-img:hover {
            transform: scale(1.05);
        }

        h1 { margin: 0; font-size: 26px; color: #222; }
        h3 { margin: 5px 0 20px 0; font-size: 16px; color: #007bff; font-weight: 500; }
        p { font-size: 15px; line-height: 1.6; color: #555; padding: 0 10px; }

        /* Desain Bagian Sertifikat */
        .cert-section {
            margin-top: 30px;
            background: #f8f9fa;
            border-radius: 8px;
            padding: 20px;
            text-align: left;
        }

        .cert-section h2 {
            font-size: 18px;
            margin-top: 0;
            border-bottom: 2px solid #ddd;
            padding-bottom: 10px;
            color: #333;
        }

        ul {
            list-style-type: none;
            padding-left: 0;
            margin: 0;
        }

        ul li {
            background: #fff;
            margin-bottom: 8px;
            padding: 10px 15px;
            border-left: 4px solid #007bff;
            border-radius: 4px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.02);
            font-size: 14px;
        }

        /* Desain Tombol JS */
        .btn-action {
            margin-top: 25px;
            padding: 12px 25px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 25px;
            cursor: pointer;
            font-size: 15px;
            font-weight: bold;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 6px rgba(0,123,255,0.2);
            width: 100%;
            max-width: 250px;
        }
        
        .btn-action:hover { 
            background-color: #0056b3; 
            transform: translateY(-2px);
        }
    </style>
</head>
<body>

    <div class="card">
        <img src="data:image/jpeg;base64,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" alt="Foto Profil" class="profile-img">
        <h1 id="userName">Muhammad Danish Athallah Sutandy</h1>
        <h3>murid</h3>
        <p>saya adalah murid sekolah  Al-kautsar, kelas 9G</p>

        <div class="cert-section">
            <h2>🏆 Sertifikat & Pencapaian</h2>
            <ul>
                    <li>Sertifikat taman kanak-kanak</li>
                    <li>Sertifikat sekolah Dasar</li>
            </ul>
        </div>
        
        <button id="contactBtn" class="btn-action">Say Hello!</button>
    </div>

    <script>
        // 1. Interaksi Klik Tombol
        const btn = document.getElementById('contactBtn');
        btn.addEventListener('click', function() {
            alert('Akses Diterima! \nTerima kasih sudah melihat portfolio Muhammad Danish Athallah Sutandy. \nMari terkoneksi dan berdiskusi seputar Cybersecurity dan Web Development!');
        });

        // 2. Interaksi Hover Profil Picture
        const img = document.querySelector('.profile-img');
        img.addEventListener('dblclick', function() {
            alert('Status Sistem: Aman. Tidak ada kerentanan terdeteksi pada profil ini.');
        });

        // 3. Efek Hacker di Console Log
        console.log('%c[+] System Secured.', 'color: #00ffcc; background: #000; font-size: 14px; padding: 2px 5px;');
        console.log('%c[+] Portfolio loaded successfully for Muhammad Danish Athallah Sutandy.', 'color: #00ffcc; background: #000; font-size: 14px; padding: 2px 5px;');
    </script>
</body>
</html>
