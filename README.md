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

        /* 文本顶部和底部居中 */
        h1, footer {
            text-align: center;
        }

        /* 表头样式 */
        header {
            background: linear-gradient(90deg, #ff9966 0%, #ff5e5e 100%);
            padding: 20px;
            text-align: center;
            color: #fff;
            margin-bottom: 30px;
        }

        /* 导航栏样式 */
        nav {
            background: #333;
            padding: 15px;
            text-align: center;
            margin-bottom: 30px;
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

        /* 模块样式 */
        .module {
            background: #fff;
            border-radius: 8px;
            padding: 20px;
            margin-bottom: 30px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .module h2 {
            color: #333;
            margin-bottom: 15px;
        }

        /* 今日重要新闻模块 */
        .news-ticker {
            background: #fff;
            border-radius: 8px;
            padding: 10px;
            margin-bottom: 30px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            overflow: hidden;
            white-space: nowrap;
        }

        .news-ticker p {
            display: inline-block;
            padding: 0 20px;
            animation: ticker 10s linear infinite;
        }

        @keyframes ticker {
            0% { transform: translateX(100%); }
            100% { transform: translateX(-100%); }
        }

        /* 作品展示模块 */
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

        /* 媒体查询（响应式设计） */
        @media (max-width: 768px) {
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
    <!-- 表头 -->
    <header>
        <h1>芮颖霄个人网站</h1>
        <p>欢迎来到我的个人网页，我是芮颖霄，热爱编程与设计，在软件开发领域深耕多年。</p>
    </header>

    <!-- 导航栏 -->
    <nav>
        <a href="#about">关于我</a>
        <a href="#resume">简历</a>
        <a href="#portfolio">作品</a>
        <a href="#news">今日新闻</a>
        <a href="#awards">荣誉奖项</a>
        <a href="#skills">技能</a>
        <a href="#contact">联系我</a>
    </nav>

    <div class="container">

        <!-- 今日重要新闻模块 -->
        <div class="news-ticker" id="news">
            <h2>今日重要新闻</h2>
            <div class="news-content">
                <p>2024年诺贝尔奖揭晓，科学家们在量子计算领域取得重大突破。</p>
                <p>全球首款可折叠手机屏幕正式发布，引领未来科技潮流。</p>
                <p>人工智能技术在医疗领域取得新进展，成功实现疾病早期诊断。</p>
            </div>
        </div>

        <!-- 关于我模块 -->
        <div class="module" id="about">
            <h2>关于我</h2>
            <p>我是芮颖霄，一名热爱编程和设计的软件工程师，专注于开发高质量的软件产品。</p>
            <img src="https://pics.umetn.com/pics/2024/10/13/1733548563411759360.jpg" alt="芮颖霄">
        </div>

        <!-- 简历模块 -->
        <div class="module" id="resume">
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

        <!-- 作品展示模块 -->
        <div class="module" id="portfolio">
            <h2>我的作品</h2>
            <div class="portfolio">
                <div class="portfolio-card">
                    <img src="https://pics.umetn.com/pics/2024/10/13/1733548563411759360.jpg" alt="项目1">
                    <h3>电商系统开发</h3>
                    <p>一套基于 SpringBoot 和 Vue.js 的电商系统，具备完整的用户管理系统和商品交易功能。</p>
                </div>
                <div class="portfolio-card">
                    <img src="https://pics.umetn.com/pics/2024/10/13/1733548563411759360.jpg" alt="项目2">
                    <h3>人工智能绘画工具</h3>
                    <p>一款基于机器学习的绘画辅助工具，能够根据用户输入的文字描述生成对应的图像。</p>
                </div>
                <div class="portfolio-card">
                    <img src="https://pics.umetn.com/pics/2024/10/13/1733548563411759360.jpg" alt="项目3">
                    <h3>类 ChatGPT 克隆项目</h3>
                    <p>实现了一个类 ChatGPT 的聊天机器人，具备智能对话功能，能够与用户进行多轮交互。</p>
                </div>
            </div>
        </div>

        <!-- 荣誉奖项模块 -->
        <div class="module" id="awards">
            <h2>荣誉奖项</h2>
            <ul>
                <li>2024年度优秀软件工程师称号</li>
                <li>2023青年创新奖</li>
                <li>2023......</li>
            </ul>
        </div>

        <!-- 技能模块 -->
        <div class="module" id="skills">
            <h2>我的技能</h2>
            <ul>
                <li>编程语言：Java, Python, JavaScript</li>
                <li>框架：SpringBoot, Vue.js, React</li>
                <li>数据库：MySQL, MongoDB</li>
                <li>工具：Git, Docker, Jenkins</li>
            </ul>
        </div>

        <!-- 行业动态模块 -->
        <div class="module">
            <h2>行业动态</h2>
            <p>2024年全球软件市场规模持续增长，人工智能和大数据技术成为主要驱动力。</p>
        </div>

        <!-- 联系我模块 -->
        <div class="module" id="contact">
            <h2>联系我</h2>
            <p>邮箱：123456@qq.com</p>
            <p>电话：13812345678</p>
        </div>
    </div>

    <!-- 页脚 -->
    <footer>
        <p>© 2024 芮颖霄个人网站 - 版权所有</p>
    </footer>
</body>
</html>
