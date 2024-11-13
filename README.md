# CSS
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pingüinito CSS</title>
  <style>
    /*General*/
    body {
      display: flex;
      justify-content: center;
      align-items: last baseline;
      height: 100vh;
      background-image:url(https://img.freepik.com/vector-gratis/paisaje-invierno-degradado_23-2149159765.jpg?t=st=1731533698~exp=1731537298~hmac=ca50c23ab8e306cfd94b035464ec5a81288287c3a82e7aadcfcc754e595a56b6&w=740);
      background-size: cover;
      background-repeat: no-repeat;
      margin: 0;
    }

    /* Cuerpo del pingüinito */
    .pinguino {
      position: relative;
      width: 200px;
      height: 250px;
      background-color: #070606;
      border-radius: 50% 50% 45% 45%;
    }

    /* centro del pinguinito */
    .pinguino::before {
      content: "";
      position: absolute;
      top: 20px;
      left: 50%;
      transform: translateX(-50%);
      width: 150px;
      height: 190px;
      background-color: #fff;
      border-radius: 50%;
    }

    /* Cabeza */
    .cabeza {
      position: absolute;
      top: -40px;
      left: 50%;
      transform: translateX(-50%);
      width: 150px;
      height: 150px;
      background-color: #070606;
      border-radius: 50%;
      z-index: 1;
    }

    /* Ojos */
    .ojo {
      position: absolute;
      top: 30px;
      width: 25px;
      height: 25px;
      background-color: #fff;
      border-radius: 50%;
    }

    .ojo.izquierdo {
      left: 25px;
    }

    .ojo.derecho {
      right: 25px;
    }

    /* Pupilas */
    .pupila {
      position: absolute;
      top: 4px;
      left: 4px;
      width: 10px;
      height: 10px;
      background-color: #333;
      border-radius: 50%;
    }

    /* Pico */
    .pico {
      position: absolute;
      top: 55px;
      left: 50%;
      transform: translateX(-50%);
      width: 20px;
      height: 15px;
      background-color: #ffab40;
      border-radius: 50% 50% 50% 50% / 40% 40% 60% 60%;
    }

    /* Alas */
    .ala {
      position: absolute;
      top: 30px;
      width: 40px;
      height: 70px;
      background-color: #070606;
      border-radius: 50%;
    }

    .ala.izquierda {
      left: -20px;
      transform: rotate(-20deg);
    }

    .ala.derecha {
      right: -20px;
      transform: rotate(20deg);
    }

    /* Pies */
    .pie {
      position: absolute;
      bottom: -10px;
      width: 40px;
      height: 30px;
      background-color: #ffab40;
      border-radius: 50% 50% 0 0;
    }

    .pie.izquierdo {
      left: 35px;
    }

    .pie.derecho {
      right: 35px;
    }
  </style>
</head>
<body>

  <div class="pinguino">
    <div class="cabeza">
      <div class="ojo izquierdo">
        <div class="pupila"></div>
      </div>
      <div class="ojo derecho">
        <div class="pupila"></div>
      </div>
      <div class="pico"></div>
    </div>
    <div class="ala izquierda"></div>
    <div class="ala derecha"></div>
    <div class="pie izquierdo"></div>
    <div class="pie derecho"></div>
  </div>

</body>
</html>