# Doraemon---css-code
A creative CSS art project recreating Doraemon using HTML and CSS, without external images.


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Doraemon CSS Art</title>

  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      display: grid;
      place-items: center;
      background: #dff6ff;
      font-family: Arial, sans-serif;
    }

    .doraemon {
      position: relative;
      width: 300px;
      height: 390px;
    }

    /* Head */
    .head {
      position: absolute;
      top: 15px;
      left: 25px;
      width: 250px;
      height: 245px;
      background: #159bd3;
      border: 5px solid #111;
      border-radius: 50% 50% 47% 47%;
      overflow: hidden;
      z-index: 3;
    }

    /* White face */
    .face {
      position: absolute;
      left: 22px;
      bottom: 8px;
      width: 196px;
      height: 185px;
      background: white;
      border: 4px solid #111;
      border-radius: 50%;
    }

    /* Eyes */
    .eye {
      position: absolute;
      top: 25px;
      width: 48px;
      height: 62px;
      background: white;
      border: 4px solid #111;
      border-radius: 50%;
      z-index: 4;
    }

    .eye.left {
      left: 77px;
    }

    .eye.right {
      left: 122px;
    }

    .eye::after {
      content: "";
      position: absolute;
      left: 17px;
      bottom: 8px;
      width: 11px;
      height: 22px;
      background: #111;
      border-radius: 50%;
    }

    /* Nose */
    .nose {
      position: absolute;
      top: 82px;
      left: 101px;
      width: 38px;
      height: 38px;
      background: #e82828;
      border: 4px solid #111;
      border-radius: 50%;
      z-index: 5;
    }

    .nose::after {
      content: "";
      position: absolute;
      top: 34px;
      left: 15px;
      width: 4px;
      height: 62px;
      background: #111;
    }

    /* Mouth */
    .mouth {
      position: absolute;
      left: 55px;
      bottom: 28px;
      width: 90px;
      height: 48px;
      border-bottom: 4px solid #111;
      border-radius: 50%;
      z-index: 5;
    }

    /* Whiskers */
    .whiskers {
      position: absolute;
      top: 127px;
      left: 0;
      width: 100%;
      height: 75px;
      z-index: 6;
    }

    .whiskers span {
      position: absolute;
      width: 65px;
      height: 3px;
      background: #111;
    }

    .whiskers .l1 {
      top: 10px;
      left: 8px;
      transform: rotate(10deg);
    }

    .whiskers .l2 {
      top: 34px;
      left: 3px;
    }

    .whiskers .l3 {
      top: 57px;
      left: 8px;
      transform: rotate(-10deg);
    }

    .whiskers .r1 {
      top: 10px;
      right: 8px;
      transform: rotate(-10deg);
    }

    .whiskers .r2 {
      top: 34px;
      right: 3px;
    }

    .whiskers .r3 {
      top: 57px;
      right: 8px;
      transform: rotate(10deg);
    }

    /* Body */
    .body {
      position: absolute;
      top: 230px;
      left: 62px;
      width: 176px;
      height: 135px;
      background: #159bd3;
      border: 5px solid #111;
      border-radius: 48% 48% 35% 35%;
      z-index: 2;
    }

    /* White belly */
    .belly {
      position: absolute;
      left: 31px;
      top: 28px;
      width: 105px;
      height: 90px;
      background: white;
      border: 4px solid #111;
      border-radius: 50%;
    }

    /* Bell */
    .bell {
      position: absolute;
      top: 12px;
      left: 66px;
      width: 48px;
      height: 42px;
      background: #ffd323;
      border: 4px solid #111;
      border-radius: 50%;
      z-index: 5;
    }

    .bell::before {
      content: "";
      position: absolute;
      left: -3px;
      top: 15px;
      width: 46px;
      height: 4px;
      background: #111;
    }

    .bell::after {
      content: "";
      position: absolute;
      left: 17px;
      bottom: 3px;
      width: 8px;
      height: 10px;
      background: #111;
      border-radius: 50%;
    }

    /* Arms */
    .arm {
      position: absolute;
      top: 255px;
      width: 58px;
      height: 30px;
      background: #159bd3;
      border: 5px solid #111;
      border-radius: 50%;
      z-index: 1;
    }

    .arm.left {
      left: 25px;
      transform: rotate(35deg);
    }

    .arm.right {
      right: 25px;
      transform: rotate(-35deg);
    }

    /* Feet */
    .foot {
      position: absolute;
      top: 343px;
      width: 82px;
      height: 42px;
      background: white;
      border: 5px solid #111;
      border-radius: 50%;
      z-index: 4;
    }

    .foot.left {
      left: 48px;
    }

    .foot.right {
      right: 48px;
    }
  </style>
</head>

<body>
  <div class="doraemon">
    <div class="arm left"></div>
    <div class="arm right"></div>

    <div class="body">
      <div class="belly"></div>
      <div class="bell"></div>
    </div>

    <div class="head">
      <div class="face"></div>

      <div class="eye left"></div>
      <div class="eye right"></div>

      <div class="nose"></div>
      <div class="mouth"></div>

      <div class="whiskers">
        <span class="l1"></span>
        <span class="l2"></span>
        <span class="l3"></span>
        <span class="r1"></span>
        <span class="r2"></span>
        <span class="r3"></span>
      </div>
    </div>

    <div class="foot left"></div>
    <div class="foot right"></div>
  </div>
</body>
</html>
