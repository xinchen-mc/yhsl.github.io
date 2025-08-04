<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>永恒森林 Minecraft 服务器</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Microsoft YaHei', 'Arial', sans-serif;
            background: url('images/banner.jpg') no-repeat center center fixed;
            background-size: cover;
            color: #ffffff;
            line-height: 1.6;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.75);
            min-height: 100vh;
            backdrop-filter: blur(5px);
        }
        header {
            text-align: center;
            padding: 40px 0;
            animation: fadeIn 1s ease-in-out;
        }
        
        header h1 {
            font-size: 3.5rem;
            color: #4CAF50;
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.8);
            margin-bottom: 15px;
            background: linear-gradient(90deg, #4CAF50, #8BC34A);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        header p {
            font-size: 1.3rem;
            color: #ddd;
            max-width: 800px;
            margin: 0 auto;
        }
        .server-info {
            background: rgba(0, 0, 0, 0.6);
            padding: 25px;
            border-radius: 12px;
            margin: 30px auto;
            text-align: center;
            max-width: 800px;
            border: 1px solid #4CAF50;
            box-shadow: 0 0 15px rgba(76, 175, 80, 0.3);
        }
        .ip-box {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }
        .ip-box span {
            font-size: 1.3rem;
            color: #eee;
        }
        #server-ip {
            font-size: 1.4rem;
            font-weight: bold;
            color: #4CAF50;
            padding: 8px 15px;
            background: rgba(0, 0, 0, 0.4);
            border-radius: 6px;
            font-family: 'Courier New', monospace;
        }
        button {
            background: linear-gradient(135deg, #4CAF50, #2E7D32);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 6px;
            cursor: pointer;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);
            background: linear-gradient(135deg, #66BB6A, #388E3C);
        }
        
        button:active {
            transform: translateY(0);
        }
        .features {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
            margin: 50px 0;
        }
        .feature-card {
            background: rgba(0, 0, 0, 0.6);
            padding: 25px;
            border-radius: 12px;
            width: 280px;
            text-align: center;
            transition: all 0.3s ease;
            border: 1px solid rgba(76, 175, 80, 0.3);
        }
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            border-color: #4CAF50;
        }
        .feature-card h3 {
            font-size: 1.5rem;
            color: #4CAF50;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        .feature-card p {
            color: #ccc;
            font-size: 1.1rem;
        }
        footer {
            text-align: center;
            margin-top: 80px;
            padding: 25px;
            color: #aaa;
            font-size: 1rem;
            border-top: 1px solid rgba(76, 175, 80, 0.2);
        }
        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }
            
            header p {
                font-size: 1.1rem;
            }
            
            .ip-box {
                flex-direction: column;
                gap: 10px;
            }
            
            .feature-card {
                width: 100%;
                max-width: 350px;
            }
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>永恒森林</h1>
            <p>一个充满魔法与冒险的纯净生存世界，探索未知的森林秘境，与好友共建梦幻家园</p>
        </header>
        
        <section class="server-info">
            <div class="ip-box">
                <span>服务器地址：</span>
                <code id="server-ip">pmt.rainplay.cn:54160</code>
                <button onclick="copyIP()">复制地址</button>
            </div>
        </section>

        <section class="features">
            <div class="feature-card">
                <h3>⚔️ 纯净生存</h3>
                <p>完全原版体验，无任何破坏平衡的插件或模组，回归Minecraft最纯粹的乐趣</p>
            </div>
            <div class="feature-card">
                <h3>🌳 特色地形</h3>
                <p>自定义生成的神秘森林生物群系，隐藏着古老遗迹和未知宝藏等你探索</p>
            </div>
            <div class="feature-card">
                <h3>🎮 友好社区</h3>
                <p>严格的玩家审核制度，24小时管理在线，打造和谐友善的游戏环境</p>
            </div>
            <div class="feature-card">
                <h3>🏰 定期活动</h3>
                <p>每周举办建筑比赛、生存挑战等丰富活动，赢取独特奖励</p>
            </div>
            <div class="feature-card">
                <h3>🔧 稳定运行</h3>
                <p>高性能服务器硬件，99.9%在线率，专业运维团队保障</p>
            </div>
            <div class="feature-card">
                <h3>📜 完善规则</h3>
                <p>清晰公平的服务器规则，保护每位玩家的游戏体验</p>
            </div>
        </section>

        <footer>
            <p>© 2023 永恒森林 Minecraft 服务器 | QQ群：123456789 | 管理员邮箱：admin@eternal-forest.com</p>
            <p>推荐使用Java版1.20.1客户端进入服务器</p>
        </footer>
    </div>

    <script>
        // 复制IP功能
        function copyIP() {
            const ip = document.getElementById('server-ip');
            navigator.clipboard.writeText(ip.innerText)
                .then(() => {
                    // 创建自定义提示框
                    const tooltip = document.createElement('div');
                    tooltip.textContent = '已成功复制服务器地址！';
                    tooltip.style.position = 'fixed';
                    tooltip.style.bottom = '20px';
                    tooltip.style.left = '50%';
                    tooltip.style.transform = 'translateX(-50%)';
                    tooltip.style.backgroundColor = '#4CAF50';
                    tooltip.style.color = 'white';
                    tooltip.style.padding = '10px 20px';
                    tooltip.style.borderRadius = '5px';
                    tooltip.style.zIndex = '1000';
                    tooltip.style.boxShadow = '0 2px 10px rgba(0,0,0,0.2)';
                    tooltip.style.animation = 'fadeInOut 2s ease-in-out';
                    
                    document.body.appendChild(tooltip);
                    
                    // 3秒后移除提示
                    setTimeout(() => {
                        tooltip.style.opacity = '0';
                        setTimeout(() => {
                            document.body.removeChild(tooltip);
                        }, 500);
                    }, 2500);
                })
                .catch(err => {
                    console.error('复制失败:', err);
                    alert('复制失败，请手动选择并复制IP地址');
                });
        }
        
        // 添加CSS动画
        const style = document.createElement('style');
        style.textContent = `
            @keyframes fadeInOut {
                0% { opacity: 0; transform: translateX(-50%) translateY(20px); }
                20% { opacity: 1; transform: translateX(-50%) translateY(0); }
                80% { opacity: 1; transform: translateX(-50%) translateY(0); }
                100% { opacity: 0; transform: translateX(-50%) translateY(-20px); }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>