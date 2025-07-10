<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Excuse Canvas - Glassmorphism</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            /* Latar belakang gradien untuk efek glassmorphism */
            background: linear-gradient(135deg, #a1c4fd 0%, #c2e9fb 100%);
        }

        .glass-container {
            /* Gaya glassmorphism */
            background: rgba(255, 255, 255, 0.15); /* Transparansi */
            backdrop-filter: blur(10px); /* Efek blur inti */
            -webkit-backdrop-filter: blur(10px); /* Kompatibilitas Safari */
            border-radius: 20px; /* Sudut membulat */
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.2); /* Bayangan */
            /* Tidak ada border */
            border: none;
            padding: 20px; /* Padding di sekitar canvas */
            display: flex;
            align-items: center;
            justify-content: center;
        }

        #quoteCanvas {
            /* Canvas akan tetap clean, tanpa border atau shadow karena sudah ditangani container */
            background: transparent; /* Pastikan canvas transparan untuk melihat efek blur di belakangnya */
            display: block; /* Menghilangkan spasi tambahan di bawah canvas */
        }
    </style>
</head>
<body>

    <div class="glass-container">
        <canvas id="quoteCanvas" width="600" height="200"></canvas>
    </div>

    <script>
        async function fetchAndDraw() {
            try {
                // Menggunakan URL Gist yang sama
                const res = await fetch("https://gist.githubusercontent.com/khoirulaksara/66a0404c464dd2ab8792cb698e999b22/raw/0fd4235dedb253ca1ec6716f9d5006c9c453819b/excused.json");
                const json = await res.json();
                const arr = json.excuses;

                if (!Array.isArray(arr) || arr.length === 0) {
                    drawText("Tidak ada alasan yang tersedia.");
                    return;
                }

                const text = arr[Math.floor(Math.random() * arr.length)];
                drawText(text);
            } catch (err) {
                console.error(err);
                drawText("Gagal memuat alasan.");
            }
        }

        function drawText(text) {
            const canvas = document.getElementById("quoteCanvas");
            const ctx = canvas.getContext("2d");
            const padding = 30; // Sedikit lebih banyak padding untuk estetika
            const maxWidth = canvas.width - padding * 2;
            const lineHeight = 30; // Sesuaikan tinggi baris
            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Gaya teks untuk tampilan yang lebih bersih
            ctx.font = "24px 'Segoe UI', sans-serif"; // Font yang lebih modern dan besar
            ctx.fillStyle = "#333"; // Warna teks gelap

            const words = text.split(" ");
            let line = "";
            let y = padding + (lineHeight / 2) + 10; // Posisi Y awal yang disesuaikan

            // Hitung tinggi teks yang dibutuhkan
            let currentLineHeight = 0;
            let lines = [];
            let tempLine = "";
            for (let n = 0; n < words.length; n++) {
                const testLine = tempLine + words[n] + " ";
                const metrics = ctx.measureText(testLine);
                if (metrics.width > maxWidth && n > 0) {
                    lines.push(tempLine);
                    tempLine = words[n] + " ";
                } else {
                    tempLine = testLine;
                }
            }
            lines.push(tempLine);

            const totalTextHeight = lines.length * lineHeight;
            const startY = (canvas.height / 2) - (totalTextHeight / 2) + (lineHeight / 2); // Pusatkan vertikal

            lines.forEach((l, index) => {
                ctx.fillText(l, padding, startY + (index * lineHeight));
            });
        }

        fetchAndDraw();
    </script>
</body>
</html>
