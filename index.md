<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .pic {
            position: relative;
        }
        .pic #img1 {
            width: 100%;
        }
        .pic a {
            display:inline-block;
            width: 100%;
            height: 65px;
        }
         .pic #img2 {
             position: absolute;
             right: 5px;
             top: 5px;
         }
    </style>
</head>
<body>
    <div class="pic">
        <a href="#" >
        <img src="./webApi-da01/5-作业/京东广告/luzhou.jpg" alt="" id="img1">
        <img src="./webApi-da01/5-作业/京东广告/close.jpg" alt="" id="img2">
        </a>
    </div>

    <script>
        var img1 = document.querySelector('#img1');
        var img2 = document.querySelector('#img2');
        var pic = document.querySelector('.pic');
        // false代表显示
        var flag = false;
        img2.onclick = function(){
            img1.style.display = flag === false ? 'none' : 'block'
            img2.src = flag === false ? "./webApi-da01/duihao.png" : "./webApi-da01/5-作业/京东广告/close.jpg"
            flag = !flag

/*             
            if(flag == false){
                img1.style.display = 'none';
                img2.src = "./webApi-da01/duihao.png";
            } else {
                img1.style.display = 'block';
                img2.src = "./webApi-da01/5-作业/京东广告/close.jpg";
            }
 */
        }

    </script>
</body>
</html>
