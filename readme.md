<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <script>
        // 获取浏览器语言
        const userLang = navigator.language || navigator.userLanguage;
        
        // 默认使用英文
        let targetFile = 'readme-en.md';
        
        // 如果语言是中文，则使用中文README
        if (userLang.startsWith('zh')) {
            targetFile = 'readme-zh.md';
        }
        
        // 跳转到对应的README文件
        window.location.href = targetFile;
    </script>
    <noscript>
        <!-- 如果用户禁用了JavaScript，显示备选方案 -->
        <meta http-equiv="refresh" content="0; url=readme-en.md">
    </noscript>
    <title>Redirecting...</title>
</head>
<body>
    <p>If you are not redirected automatically, follow these links:</p>
    <ul>
        <li><a href="readme-en.md">English Version</a></li>
        <li><a href="readme-zh.md">中文版本</a></li>
    </ul>
</body>
</html>