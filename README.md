<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>芮颖霄个人网站</title>
    <style>
        /* 全局样式 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background: linear-gradient(135deg, #f5f7fa 0%, #e3e8f0 100%);
            color: #333;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* 导航栏样式 */
        nav {
            background: #333;
            padding: 15px;
            text-align: center;
        }

        nav a {
            text-decoration: none;
            color: #fff;
            font-size: 18px;
            margin: 0 20px;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* 主页横幅 */
        .hero {
            background: url('https://images.unsplash.com/photo-1586901294113-4fd78b44e9de?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTB8fGFwcGxpY2F0aW9ufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60') center center / cover no-repeat;
            color: #fff;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 400px;
            margin-bottom: 30px;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            max-width: 600px;
        }

        /* 简历模块 */
        .resume-module {
            background: #fff;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 30px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .resume-module h2 {
            color: #333;
            margin-bottom: 15px;
        }

        .education, .work-experience {
            margin-bottom: 20px;
        }

        /* 作品展示 */
        .portfolio {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .portfolio-card {
            background: #fff;
            border-radius: 8px;
            padding: 15px;
            overflow: hidden;
            flex-basis: calc(33.333% - 20px);
            transition: transform 0.3s ease;
        }

        .portfolio-card:hover {
            transform: translateY(-10px);
        }

        .portfolio-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .portfolio-card h3 {
            font-size: 20px;
            color: #333;
            margin-bottom: 10px;
        }

        /* 宣传横幅 */
        .ad-banner {
            background: linear-gradient(90deg, #ff9966 0%, #ff355e 100%);
            padding: 20px;
            text-align: center;
            margin-bottom: 30px;
            color: #fff;
        }

        .ad-banner h2 {
            font-size: 24px;
        }

        /* 版权和联系信息 */
        .contact-info {
            background: #333;
            color: #fff;
            text-align: center;
            padding: 15px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        .contact-info a {
            color: #fff;
            text-decoration: none;
        }

        .contact-info a:hover {
            text-decoration: underline;
        }

        /* 媒体查询（响应式设计） */
        @media (max-width: 768px) {
            .hero {
                height: 300px;
                padding: 20px;
            }

            .hero h1 {
                font-size: 28px;
            }

            .portfolio-card {
                flex-basis: 100%;
            }
        }

        @media (max-width: 480px) {
            body {
                font-size: 14px;
            }

            .portfolio-card img {
                height: 150px;
            }
        }
    </style>
</head>
<body>
    <!-- 主页横幅 -->
    <div class="hero container">
        <h1>芮颖霄个人网页</h1>
        <p>欢迎来到我的个人网页，我是芮颖霄，热爱编程与设计，在软件开发领域深耕多年。</p>
    </div>

    <!-- 导航栏 -->
    <nav class="container">
        <a href="#resume">简历</a>
        <a href="#portfolio">作品</a>
        <a href="#awards">荣誉奖项</a>
        <a href="#contact">联系我</a>
    </nav>

    <div class="container">

        <!-- 高端横幅（宣传广告） -->
        <div class="ad-banner">
            <h2>浏览我的作品，寻找灵感！</h2>
            <p>更多精美作品，安装后即可查看</p>
        </div>

        <!-- 简历模块 -->
        <div class="resume-module" id="resume">
            <h2>我的简历</h2>

            <div class="education">
                <h3>教育背景</h3>
                <p><strong>浙江科技学院</strong> - 软件工程专业 - 2020-2024</p>
                <p>主修课程包括Java编程、数据结构与算法、软件工程等，积极参与学校组织的开发活动。</p>
            </div>

            <div class="work-experience">
                <h3>工作经历</h3>
                <p><strong>ABC科技有限公司</strong> - 软件开发工程师 - 2024-至今</p>
                <ul>
                    <li>开发维护公司核心产品。</li>
                </ul>
            </div>
        </div>

        <!-- 作品展示 -->
        <section id="portfolio">
            <h2 class="text-center">我的作品</h2>

            <div class="portfolio">
                <div class="portfolio-card">
                    <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="项目1">
                    <h3>电商系统开发</h3>
                    <p>一套基于 SpringBoot 和 Vue.js 的电商系统，具备完整的用户管理系统和商品交易功能。</p>
                </div>

                <div class="portfolio-card">
                    <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="项目2">
                    <h3>人工智能绘画工具</h3>
                    <p>一款基于机器学习的绘画辅助工具，能够根据用户输入的文字描述生成对应的图像。</p>
                </div>

                <div class="portfolio-card">
                    <img src="https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt="项目3">
                    <h3>类 ChatGPT 克隆项目</h3>
                    <p>实现了一个类 ChatGPT 的聊天机器人，具备智能对话功能，能够与用户进行多轮交互。</p>
                </div>
            </div>
        </section>
        
        <!-- 荣誉奖项 -->
        <section id="awards">
            <h2>荣誉奖项</h2>
            <ul>
                <li>2024年度优秀软件工程师称号</li>
                <li>2023青年创新奖</li>
                <li>2023......</li>
            </ul>
        </section>
    </div>

    <!-- 联系信息 -->
    <footer class="contact-info">
        <p>联系邮箱：123456@qq.com</p>
        <p>电话：1381234567</p>
        <p>版权所有 © 2025-2099 版权所有，仿冒必究</p>
    </footer>
</body>
</html>
