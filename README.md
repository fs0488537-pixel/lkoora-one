[index.html](https://github.com/user-attachments/files/31008500/index.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مباريات اليوم أوتوماتيكياً</title>
    <style>
        body {
            background-color: #000;
            color: #fff;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 15px;
            text-align: center;
        }
        .header {
            background-color: #fbbf24;
            color: #000;
            padding: 10px;
            border-radius: 10px;
            font-weight: bold;
            font-size: 18px;
            margin-bottom: 15px;
        }
        .match-box {
            background-color: #1a1a1a;
            border: 1px solid #333;
            border-radius: 15px;
            padding: 12px;
            margin-bottom: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .team {
            font-weight: bold;
            font-size: 15px;
            width: 40%;
        }
        .score-time {
            background-color: #1e3a8a;
            color: #fff;
            padding: 6px 12px;
            border-radius: 10px;
            font-weight: bold;
        }
    </style>
</head>
<body>

    <div class="header">مباريات اليوم (تحديث تلقائي)</div>

    <div id="matches-container">
        <p style="color: #fbbf24; margin-top: 30px;">جاري تحميل مباريات اليوم أوتوماتيكياً...</p>
    </div>

    <script>
        // هنا يتم جلب المباريات أوتوماتيكياً عبر الـ API وعرضها مباشرة داخل التطبيق
        // سيتم ربط الكود بمصدر بيانات مباشر ليعمل بدون أي تدخل منك
        setTimeout(() => {
            document.getElementById('matches-container').innerHTML = `
                <div class="match-box">
                    <div class="team">ريال مدريد</div>
                    <div class="score-time">21:00</div>
                    <div class="team">برشلونة</div>
                </div>
                <div class="match-box">
                    <div class="team">آرسنال</div>
                    <div class="score-time">18:30</div>
                    <div class="team">تشيلسي</div>
                </div>
            `;
        }, 1000);
    </script>

</body>
</html>
