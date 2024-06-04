- 👋 Hi, I’m Aasta
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aasta的個人網站</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('https://example.com/nature-background.jpg'); /* 替換為自然風景圖片的URL */
            background-size: cover;
            color: #333;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
        }
        .logo {
            text-align: center;
        }
        .logo img {
            max-width: 150px;
        }
        .header {
            text-align: center;
            padding: 20px 0;
        }
        .header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        .about, .portfolio {
            margin: 20px 0;
        }
        .portfolio img {
            max-width: 100%;
            height: auto;
        }
        .add-work {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            cursor: pointer;
            text-align: center;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="logo">
            <img src="file-HdgzAuymNt9God4YgXlQJarM" alt="Aasta的Logo">
        </div>
        <div class="header">
            <h1>Aasta的個人網站</h1>
        </div>
        <div class="about">
            <h2>個人簡介</h2>
            <p>大家好！我是Aasta，我的興趣是畫畫。我喜歡創造和分享我的藝術作品。歡迎來到我的個人網站！</p>
        </div>
        <div class="portfolio">
            <h2>作品集</h2>
            <div id="works">
                <!-- 這裡是作品展示區域 -->
            </div>
            <button class="add-work" onclick="addWork()">新增作品</button>
        </div>
    </div>
    <script>
        function addWork() {
            const worksDiv = document.getElementById('works');
            const workDescription = prompt('請輸入作品描述:');
            const workImageUrl = prompt('請輸入作品圖片的URL:');

            if (workDescription && workImageUrl) {
                const workElement = document.createElement('div');
                workElement.innerHTML = `
                    <h3>${workDescription}</h3>
                    <img src="${workImageUrl}" alt="${workDescription}">
                `;
                worksDiv.appendChild(workElement);
            } else {
                alert('描述和圖片URL不能為空！');
            }
        }
    </script>
</body>
</html>
