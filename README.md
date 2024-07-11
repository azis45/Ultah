<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>

    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-image: url(Poto/poto\ 4.jpg);
        }
        
        h1{
            color: #fff;
        }

        #btn-alert {
            border: none;
            border-radius: 5px;
            padding: 7px 10px;
            background-color:hotpink;
            font-size: 1.3em;
            color: #fff;
            cursor: pointer;
            transition: 0.2s;
            position: fixed;
            left: 45%;
            top: 45%;
        }
        
        #btn-alert:hover {
            opacity: 0.8;
        }
        
        #btn-alert:focus {
            outline: rgb(37, 116, 226) solid 3px;
            outline-offset: 3px; 
        }
        
        @media (max-width: 576px) {
            #btn-alert {
                left: 38%;
            }
        }
    </style>

    <title>Happy Birthday Honey</title>
</head>

<body>
<H1>Penasaran yahhh</H1>
    <button id="btn-alert" onclick="munculinAlert()">ayoo klik!</button>

    <script>
        async function munculinAlert() {
            await Swal.fire('Holaaa Dea Ananda Nurlijani 💓❣💖🤍💕🎉✨')
            await Swal.fire('Selamat ulang tahun yaa... cintakuu')
            await Swal.fire({
                title: 'Selamat ulang tahun di usia ke - 19 saayangghkuuu ',
                text: 'Semoga panjang umur, sehat selalu dan semoga dilancarkan segala nya yahh... cantikkuu😉',
                imageUrl: 'Poto/poto 1.jpg',
                imageWidth: 400,
                imageHeight: 300,
                imageAlt: 'Gambar kue ulang tahun',
            })
            await Swal.fire({
                title: 'Suka atau Tidak Suka',
                text: "Tolong jawab yang jujur ya... bahagiakuuu",
                icon: 'question',
                showDenyButton: true,
                confirmButtonColor: '#3085d6',
                confirmButtonText: 'Hmm suka dan keren 😎',
                denyButtonText: `kayaknya aku kurang suka 😕`,
            }).then((result) => {
                if (result.isConfirmed) {
                    Swal.fire({
                        title: 'Horee Berhasil',
                        text: 'Terimakasih banyak sayanggkuu, maaf banget yahh aku cuman bisa ngasih ini buat kamu ayanggkuu, semoga berkesan ^_^',
                        imageUrl: 'Poto/poto 2.jpg',
                        imageWidth: 400,
                        imageHeight: 300,
                        imageAlt: 'Gambar Gojo bahagia',
                    })
                } else {
                    Swal.fire({
                        title: 'Yahhh gagal 😔',
                        text: 'Yah, maaf banget ni kalau ga suka 😢',
                        imageUrl: 'Poto/poto 3.jpg',
                        imageWidth: 400,
                        imageHeight: 300,
                        imageAlt: 'Gambar Anime sedih',
                    })
                }
            })
        }
    </script>

</body>

</html>
