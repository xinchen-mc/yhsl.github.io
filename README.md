# yhsl.github.io
永恒森林服务器官网
eternal-forest/
├── index.html          # 主页面
├── style.css           # 样式
└── images/
    └── banner.png      # 背景图（需自行上传）

<!DOCTYPE html>
<html>
<head>
    <title>永恒森林 Minecraft 服务器</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <div class="container">
        <header>
            <h1>永恒森林</h1>
            <p>一个充满魔法与冒险的纯净生存世界</p>
        </header>
        
        <section class="server-info">
            <div class="ip-box">
                <span>服务器地址：</span>
                <code id="server-ip">pmt.rainplay.cn:54160</code>
                <button onclick="copyIP()">复制</button>
            </div>
        </section>

        <section class="features">
            <div class="feature-card">
                <h3>⚔️ 纯净生存</h3>
                <p>无作弊、无付费特权，回归原版乐趣</p>
            </div>
            <div class="feature-card">
                <h3>🌳 特色地形</h3>
                <p>自定义生成魔法森林与地下城</p>
            </div>
            <div class="feature-card">
                <h3>🎮 友好社区</h3>
                <p>禁止熊孩子，共建和谐世界</p>
            </div>
        </section>

        <footer>
            <p>© 2023 永恒森林 · QQ群：123456789</p>
        </footer>
    </div>

    <script>
        function copyIP() {
            const ip = document.getElementById('server-ip');
            navigator.clipboard.writeText(ip.innerText);
            alert('已复制IP: ' + ip.innerText);
        }
    </script>
</body>
</html>
body {
    font-family: 'Arial', sans-serif;
    background: url('images/banner.png') no-repeat center center fixed;
    background-size: cover;
    color: white;
    margin: 0;
    padding: 0;
}

.container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    background-color: rgba(0, 0, 0, 0.7);
    min-height: 100vh;
}

header {
    text-align: center;
    padding: 40px 0;
}

h1 {
    font-size: 3em;
    color: #4CAF50;
    text-shadow: 2px 2px 4px #000;
}

.server-info {
    background: rgba(0, 0, 0, 0.5);
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
    text-align: center;
}

.ip-box {
    font-size: 1.2em;
}

button {
    background: #4CAF50;
    color: white;
    border: none;
    padding: 8px 15px;
    border-radius: 5px;
    cursor: pointer;
    margin-left: 10px;
}

.features {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: center;
}

.feature-card {
    background: rgba(0, 0, 0, 0.5);
    padding: 15px;
    border-radius: 10px;
    width: 200px;
    text-align: center;
}

footer {
    text-align: center;
    margin-top: 50px;
    padding: 20px;
}