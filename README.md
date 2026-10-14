<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>奶龙</title>
    <meta http-equiv="refresh" content="5; url=https://www.scitc.edu.cn/">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background-color: #FFEB3B;
            background-image: radial-gradient(circle, #FFEB3B 0%, #FFC107 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: "Microsoft YaHei", sans-serif;
            overflow: hidden;
        }
        .container {
            text-align: center;
            animation: floaty 3s ease-in-out infinite;
        }
        @keyframes floaty {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
        .nailong {
            width: 400px;
            max-width: 80vw;
            filter: drop-shadow(0 20px 30px rgba(0,0,0,0.2));
        }
        .title {
            font-size: 36px;
            color: #E65100;
            margin-top: 30px;
            font-weight: bold;
            text-shadow: 2px 2px 0 #FFF;
        }
        .subtitle {
            font-size: 20px;
            color: #BF360C;
            margin-top: 10px;
        }
        .countdown {
            font-size: 18px;
            color: #E65100;
            margin-top: 20px;
        }
        .countdown span {
            font-size: 28px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <img class="nailong" src=""C:\Users\35936\Desktop\OIP-C (1).webp"" alt="奶龙">
        <div class="title">奶龙</div>
        <div class="subtitle">我才不是胖橘~</div>
        <div class="countdown">页面将在 <span id="sec">5</span> 秒后跳转到四川信息职业技术学院官网</div>
    </div>
    <script>
        var sec = 5;
        var timer = setInterval(function() {
            sec--;
            document.getElementById('sec').innerText = sec;
            if (sec <= 0) clearInterval(timer);
        }, 1000);
    </script>
</body>
</html>
