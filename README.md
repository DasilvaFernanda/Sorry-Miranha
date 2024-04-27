# Sorry-Miranha
Pedido de desculpas ao meu amigo que gosta do miranha
!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eu gosto muito de vc</title>

    <style>
        body{
            background-color: rgb(80, 8, 80);
        }

        .painel{
            margin: auto;
            background-color: white;
            width: 500px;
            height: 700px;
            border-radius: 20px;
            text-align: center;
            padding-top: 50px;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }
        #sim{
            height: 40px;
            width: 60px;
            background-color: rgb(35, 59, 196);
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: -50px;
        }
        #nao{
            position: absolute;
            height: 40px;
            width: 60px;
            background-color: red;
            border: 2px solid white;
            border-radius: 10px;
            color: white;
            margin-left: 10px;
        }

    </style>

</head>
<body>

    <div class="painel">
        <h1> Oi Jubileu </h1>

        <img src="https://media1.tenor.com/m/8i5q-Hu-4RIAAAAC/spiderman-superhero.gif" alt="">

        <h2>você perdoaria a pipoquinha na manteiga?</h2>
        

        <a href="https://www.youtube.com/watch?v=C3KinLVXX5A"><button id="sim" > Sim! </button></a>
        <button onmouseover="fuja()" id="nao"> Não! </button>
        
    </div>

    <script>
        function fuja(){
            var botaoNao = document.getElementById("nao")

            var larguraJanela = window.innerWidth;
            var alturaJanela = window.innerHeight;

            var maxX = larguraJanela - botaoNao.offsetWidth;
            var maxY = alturaJanela - botaoNao.offsetHeight;

            var aleatorioX = Math.floor(Math.random() * maxX);
            var aleatorioY = Math.floor(Math.random() * maxY);

            botaoNao.style.left = aleatorioX + "px";
            botaoNao.style.top = aleatorioY + "px";


        }
    </script>



    
</body>
</html>
