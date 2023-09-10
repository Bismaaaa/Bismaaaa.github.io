<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://fonts.googleapis.com/css?family=Indie+Flower" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css?family=Amatic+SC" rel="stylesheet">
    <style>
        /* CSS Styles */
        @import url('https://fonts.googleapis.com/css?family=Indie+Flower');
        @import url('https://fonts.googleapis.com/css?family=Amatic+SC');

        body {
            font-family: 'Indie Flower', cursive !important;
            background: #FDE3A7;
            margin: 0px;
            padding: 0px;
        }

        ::selection {
            background: transparent;
        }

            h4.color1 {
                font-size: 35px;
                font-family: 'Amatic SC', cursive !important;
                margin-bottom: 5px;
                /* Sesuaikan nilai ini sesuai dengan seberapa dekat Anda ingin elemen pertama dengan elemen kedua */
            }

            h4.color2 {
                font-size: 35px;
                font-family: 'Amatic SC', cursive !important;
                margin-top: -5px;
                /* Sesuaikan nilai ini sesuai dengan seberapa dekat Anda ingin elemen kedua dengan elemen pertama */
            }


        p {
            font-size: 7px;
        }

        .color1 {
            color: #1BBC9B;
        }

        .color2 {
            color: #C0392B;
        }

        .card {
            color: #013243;
            position: absolute;
            top: 50%;
            left: 50%;
            width: 300px;
            height: auto;
            /* Menggunakan auto agar tinggi kartu menyesuaikan kontennya */
            background: #e0e1dc;
            transform-style: preserve-3d;
            transform: translate(-50%, -50%) perspective(200px);
            box-shadow: inset 300px 0 50px rgba(0, 0, 0, .5), 20px 0 60px rgba(0, 0, 0, .5);
            transition: .1s;
        }

        .card:hover {
            transform: translate(-50%, -50%) perspective(2000px) rotate(15deg) scale(1.2);
            box-shadow: inset 20px 0 50px rgba(0, 0, 0, .5), 0 10px 100px rgba(0, 0, 0, .5);
        }

        .card::before {
            content: '';
            position: absolute;
            top: -5px;
            left: 0;
            width: 100px;
            height: 5px;
            background: #BAC1BA;
            transform-origin: bottom;
            transform: skewX(-45deg);
        }

        .card::after {
            content: '';
            position: absolute;
            top: 0;
            right: -5px;
            width: 5px;
            height: 100%;
            background: #92A29C;
            transform-origin: left;
            transform: skewY(-45deg);
        }

        .card .imgBox {
            width: 100%;
            height: 100%;
            position: relative;
            transform-origin: left;
            transition: .7s;
        }

        .card .bark {
            position: absolute;
            background: #e0e1dc;
            width: 100%;
            height: 100%;
            opacity: 0;
            transition: .7s;
        }

        .card .imgBox img {
            max-width: 100%;
            /* Lebar maksimum gambar mengikuti lebar kontainer */
            max-height: 100%;
            /* Tinggi maksimum gambar mengikuti tinggi kontainer */
        }

        .card:hover .imgBox {
            transform: rotateY(-135deg);
        }

        .card:hover .bark {
            opacity: 1;
            transition: .6s;
            box-shadow: 300px 200px 100px rgba(0, 0, 0, .4) inset;
        }

        .card .details {
            position: absolute;
            top: 0;
            left: 0;
            box-sizing: border-box;
            padding: 2px;
            /* Padding tambahan untuk konten */
            z-index: -1;
            margin-top: -5px;
        }

        .card .details h4 {
            text-align: center;
        }

        .text-right {
            text-align: right;
        }
    </style>
    <title>Cipcippp Lagi Ultah</title>
</head>

<body>
    <div class="card">
        <div class="imgBox">
            <div class="bark"></div>
            <img src="/Users/bismaaa/Documents/Bahan Belajar/20230910_101401.jpg" alt="" srcset="">
        </div>
        <div class="details">
            <h4 class="color1">Happy Birthday!</h4>
            <h4 class="color2">Cipcippp</h4>
            <p>Dear Cipcippp,</p>
            <p>Makasihh ya udah mau bukak....</p>
            <p>have a great Birthday yg ke-19 yaaaa, ga sadar udah last teen aja nihh</p>
            <p>maap hadiahnya sederhana banget ya hehee, aku ngga pandai buat kata" mutiara,mungkin</p>
            <p> di surat sederhana ini aku cuma ngasi doa aja yaa, Semoga di umurmu yg sekarang kamu bisa lebih</p>
            <p>dewasa,lebih bijaksana,dan lebih peduli terhadap diri kamu sendiri yaa,maupun sekitar mu</p>
            <p>jaga kesehatan ga ada yg peduli selain dirimu sendiri,semoga segala rintangan dapat</p>
            <p>kamu lewati dengan senyuman dan ketabahan hati,semoga di jauhkan dari orang" negatif</p>
            <p>dan yang paling penting Semoga kuliah nya lancar kaya jalan tol kalo ga macet</p>
            <p> selebihnya doa sendiri yaa dah besarr jangan manja hehee</p>

            <p class="text-right">Happy Birthday , my fav Human</p>
        </div>
    </div>
    <script>
        // JavaScript
        // Fungsi untuk menampilkan pesan ucapan ulang tahun
        function showMessage() {
            alert("Selamat Ulang Tahun, Cipcippp! Semoga hari ulang tahunmu penuh kebahagiaan!");
        }

        // Mengambil elemen dengan class "color1" dan mengubah warnanya
        const color1Element = document.querySelector(".color1");
        color1Element.style.color = "#1BBC9B";

        // Mengambil elemen dengan class "color2" dan mengubah warnanya
        const color2Element = document.querySelector(".color2");
        color2Element.style.color = "#C0392B";

        // Memanggil fungsi showMessage() saat halaman dimuat
        window.onload = showMessage;
    </script>
</body>

</html>
