/* 基础样式重置 */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary-color: #4CAF50;
    --secondary-color: #2E7D32;
    --text-color: #f5f5f5;
    --dark-bg: rgba(0, 0, 0, 0.7);
    --card-bg: rgba(30, 30, 30, 0.8);
    --section-padding: 4rem 0;
}

body {
    font-family: 'Microsoft YaHei', 'PingFang SC', sans-serif;
    color: var(--text-color);
    line-height: 1.6;
    background-color: #121212;
    background-image: url('images/banner.jpg');
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
}

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* 导航栏样式 */
.navbar {
    background-color: var(--dark-bg);
    backdrop-filter: blur(5px);
    position: fixed;
    width: 100%;
    z-index: 1000;
    padding: 1rem 0;
    border-bottom: 1px solid rgba(76, 175, 80, 0.3);
}

.logo {
    display: flex;
    align-items: center;
    text-decoration: none;
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
}

.logo img {
    height: 40px;
    margin-right: 10px;
}

.nav-links {
    display: flex;
    gap: 2rem;
}

.nav-links a {
    color: var(--text-color);
    text-decoration: none;
    transition: color 0.3s;
}

.nav-links a:hover {
    color: var(--primary-color);
}

/* 英雄区域 */
.hero {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.8));
    padding-top: 80px;
}

.hero-content {
    max-width: 800px;
    padding: 0 20px;
}

.hero h1 {
    font-size: 3.5rem;
    margin-bottom: 1rem;
    background: linear-gradient(90deg, #4CAF50, #8BC34A);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.hero p {
    font-size: 1.5rem;
    margin-bottom: 2rem;
}

.server-ip {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    margin-top: 2rem;
    flex-wrap: wrap;
}

.server-ip span {
    font-size: 1.2rem;
}

.server-ip code {
    font-family: 'Courier New', monospace;
    font-size: 1.3rem;
    background: rgba(0, 0, 0, 0.5);
    padding: 0.5rem 1rem;
    border-radius: 5px;
    border: 1px solid var(--primary-color);
}

button, .qq-btn, .social-btn {
    background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
    color: white;
    border: none;
    padding: 0.8rem 1.5rem;
    border-radius: 5px;
    cursor: pointer;
    font-size: 1rem;
    transition: all 0.3s;
    text-decoration: none;
    display: inline-block;
}

button:hover, .qq-btn:hover, .social-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(76, 175, 80, 0.4);
}

/* 内容区域 */
.section {
    padding: var(--section-padding);
    background-color: var(--dark-bg);
    margin: 2rem 0;
    border-radius: 10px;
    backdrop-filter: blur(5px);
}

.section h2 {
    font-size: 2.5rem;
    margin-bottom: 2rem;
    color: var(--primary-color);
    text-align: center;
}

/* 关于区域 */
.about-content {
    display: flex;
    gap: 3rem;
    align-items: center;
}

.about-text {
    flex: 1;
}

.about-text p {
    margin-bottom: 1rem;
    font-size: 1.1rem;
    line-height: 1.8;
}

.about-image {
    flex: 1;
}

.about-image img {
    width: 100%;
    border-radius: 8px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
}

/* 特色区域 */
.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
}

.feature-card {
    background: var(--card-bg);
    padding: 2rem;
    border-radius: 10px;
    transition: all 0.3s;
    border: 1px solid rgba(76, 175, 80, 0.1);
}

.feature-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
    border-color: var(--primary-color);
}

.feature-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
}

.feature-card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: var(--primary-color);
}

/* 规则区域 */
.rules-list {
    display: flex;
    gap: 3rem;
    justify-content: center;
    flex-wrap: wrap;
}

.rule-item {
    flex: 1;
    min-width: 300px;
    background: var(--card-bg);
    padding: 2rem;
    border-radius: 10px;
}

.rule-item h3 {
    font-size: 1.5rem;
    margin-bottom: 1.5rem;
    color: var(--primary-color);
    border-bottom: 1px solid rgba(76, 175, 80, 0.3);
    padding-bottom: 0.5rem;
}

.rule-item ul {
    list-style-position: inside;
}

.rule-item li {
    margin-bottom: 0.8rem;
    font-size: 1.1rem;
}

/* 加入区域 */
.join-methods {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
}

.join-card {
    background: var(--card-bg);
    padding: 2rem;
    border-radius: 10px;
    text-align: center;
}

.join-card h3 {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: var(--primary-color);
}

.join-card p {
    margin-bottom: 1.5rem;
}

.qq-group {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    align-items: center;
}

.social-links {
    display: flex;
    gap: 1rem;
    justify-content: center;
}

/* 页脚 */
footer {
    background: var(--dark-bg);
    padding: 3rem 0;
    margin-top: 3rem;
    border-top: 1px solid rgba(76, 175, 80, 0.3);
}

.footer-content {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

.footer-logo {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;
    font-size: 1.5rem;
    font-weight: bold;
}

.footer-logo img {
    height: 50px;
}

.footer-links {
    display: flex;
    justify-content: center;
    gap: 2rem;
    flex-wrap: wrap;
}

.footer-links a {
    color: var(--text-color);
    text-decoration: none;
    transition: color 0.3s;
}

.footer-links a:hover {
    color: var(--primary-color);
}

.footer-info {
    text-align: center;
    color: #aaa;
    font-size: 0.9rem;
}

/* 响应式设计 */
@media (max-width: 768px) {
    .hero h1 {
        font-size: 2.5rem;
    }
    
    .hero p {
        font-size: 1.2rem;
    }
    
    .about-content {
        flex-direction: column;
    }
    
    .nav-links {
        gap: 1rem;
    }
    
    .section {
        padding: 3rem 0;
    }
}

/* 动画效果 */
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.section {
    animation: fadeIn 0.8s ease-out;
}