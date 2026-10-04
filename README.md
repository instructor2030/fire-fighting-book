<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الحقيبة التدريبية الإلكترونية - الإطفاء والإنقاذ</title>
    <style>
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #18bc9c;
            --accent-color: #e74c3c;
            --dark-blue: #1a252f;
            --light-bg: #f8f9fa;
            --border-color: #e2e8f0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--light-bg);
            color: #333;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--dark-blue), var(--primary-color));
            color: white;
            padding: 40px 20px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.15);
            position: relative;
        }

        header h1 {
            margin: 0;
            font-size: 2.2rem;
            font-weight: 700;
            letter-spacing: 0.5px;
        }

        header p {
            margin: 10px 0 0 0;
            font-size: 1.1rem;
            opacity: 0.9;
        }

        .search-wrapper {
            max-width: 650px;
            margin: -25px auto 30px auto;
            padding: 0 20px;
            position: relative;
            z-index: 10;
        }

        #searchInput {
            width: 100%;
            padding: 16px 25px;
            font-size: 17px;
            border: none;
            border-radius: 50px;
            box-sizing: border-box;
            outline: none;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            text-align: center;
        }

        #searchInput:focus {
            box-shadow: 0 4px 25px rgba(24, 188, 156, 0.3);
            transform: scale(1.01);
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px 50px 20px;
        }

        .part-title {
            font-size: 1.5rem;
            color: var(--dark-blue);
            margin: 40px 0 20px 0;
            padding-right: 15px;
            border-right: 5px solid var(--accent-color);
        }

        .section-card {
            background: white;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
        }

        .section-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 15px rgba(0,0,0,0.05);
        }

        h3 {
            color: var(--primary-color);
            margin-top: 0;
            font-size: 1.35rem;
            border-bottom: 2px solid var(--light-bg);
            padding-bottom: 12px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .unit-badge {
            background-color: var(--secondary-color);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 13px;
            font-weight: normal;
        }

        h4 {
            color: var(--accent-color);
            margin: 20px 0 10px 0;
            font-size: 1.1rem;
        }

        p, ul {
            color: #555;
            font-size: 15px;
        }

        ul {
            padding-right: 20px;
            list-style-type: square;
        }

        li {
            margin-bottom: 8px;
        }

        .media-box {
            margin-top: 25px;
            background: var(--light-bg);
            border-radius: 8px;
            padding: 15px;
            border: 1px dashed #cbd5e1;
        }

        .video-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.08);
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
        }

        .video-title {
            font-size: 14px;
            color: var(--primary-color);
            margin-bottom: 10px;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .no-results {
            text-align: center;
            color: var(--accent-color);
            font-size: 18px;
            display: none;
            padding: 40px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1-fr));
            gap: 15px;
            margin-top: 15px;
        }

        .info-item {
            background: var(--light-bg);
            padding: 12px;
            border-radius: 6px;
            border-right: 4px solid var(--secondary-color);
        }
    </style>
</head>
<body>

<header>
    <h1>حقيبة الإطفاء والإنقاذ التدريبية التفاعلية</h1>
    <p>المديرية العامة للدفاع المدني - المملكة العربية السعودية</p>
</header>

<div class="search-wrapper">
    <input type="text" id="searchInput" onkeyup="liveSearch()" placeholder="🔍 ابحث عن أي كلمة، وحدة، أو أداة داخل الكتاب الفني...">
</div>

<div class="container" id="bookContent">
    <div class="no-results" id="noResults">❌ عذراً، لم نجد أي محتوى يطابق بحثك. جرب كلمات أخرى مثل (طفاية، خوذة، حبل، تنفس).</div>

    <!-- الجزء الأول -->
    <div class="part-group">
        <div class="part-title">الجزء الأول: معدات الوقاية الفردية</div>

        <!-- الوحدة الأولى -->
        <div class="section-card">
            <h3>الوحدة الأولى: تعريف تجهيزات ومعدات الوقاية الفردية <span class="unit-badge">الوحدة 1</span></h3>
            <p><strong>المفهوم الفني:</strong> هي معدات وأدوات وإجراءات وقائية تُستخدم لحماية رجل الدفاع المدني من الإصابات والأضرار البدنية والمخاطر التي قد تفاجئه أثناء مباشرة أعماله الميدانية.</p>
            <h4>الشروط الواجب توفرها في المعدات:</h4>
            <ul>
                <li>أن تكون مطابقة للمواصفات الفنية والتصنيفات العالمية.</li>
                <li>أن تكون فعالة ومناسبة للجسم ومريحة وسهلة الاستخدام لضمان حرية الحركة.</li>
                <li>أن تتحمل ظروف العمل القاسية بحيث يطول عمرها الافتراضي.</li>
            </ul>
            <div class="media-box">
                <div class="video-title">📺 فيديو تعليمي: مقدمة عن معدات الوقاية الشخصية لرجال الإطفاء</div>
                <div class="video-container">
                    <iframe src="https://youtube.com" allowfullscreen></iframe>
                </div>
            </div>
        </div>

        <!-- الوحدة الثانية -->
        <div class="section-card">
            <h3>الوحدة الثانية: أجزاء تجهيزات ومعدات الوقاية الفردية <span class="unit-badge">الوحدة 2</span></h3>
            <p>يتكون لباس رجل الإطفاء من أجزاء أساسية متكاملة هندسياً لحمايته بالكامل:</p>
            <div class="info-grid">
                <div class="info-item"><strong>البدلة الواقية:</strong> مصنوعة من مواد تقاوم الحريق وتتحمل البيئات الخطرة لحماية الجسم بالكامل.</div>
                <div class="info-item"><strong>الخوذة (حماية الرأس):</strong> من الأساسيات الميدانية لحماية الرأس من صدمات الأجسام الصلبة الساقطة.</div>
                <div class="info-item"><strong>غطاء الرأس (القلنسوة):</strong> قماش يقاوم اللهب يلبس تحت الخوذة لتغطية الرقبة والأذنين وأطراف الوجه.</div>
                <div class="info-item"><strong>الحذاء الواقي:</strong> يتميز بقدرته على الحماية من سقوط المواد، عزل التيار الكهربائي، ومقاومة الانزلاق والمواد الكيميائية.</div>
                <div class="info-item"><strong>النظارة والقفازات:</strong> حماية العين من الشرر والأتربة، وحماية اليدين من الجروح القطعية والصدمات الكهربائية.</div>
                <div class="info-item"><strong>الكمامة الواقية:</strong> قناع بمرشح للأماكن التي لا تزيد نسبة الغازات والدخان فيها عن (1%).</div>
            </div>
        </div>

        <!-- الوحدة الثالثة -->
        <div class="section-card">
            <h3>الوحدة الثالثة: جهاز التنفس <span class="unit-badge">الوحدة 3</span></h3>
            <p><strong>تعريف الجهاز:</strong> جهاز يعتمد على الهواء المضغوط، ويستخدمه رجال الإطفاء والإنقاذ للعمل في الأماكن المليئة بالدخان أو الغازات السامة أو نقص الأكسجين.</p>
            <p><strong>طريقة عمله:</strong> تكون الأسطوانة بضغط عالٍ (300 بار)، يمر الهواء عبر نظام خفض الضغط ليقل إلى (7-9 بار)، ثم يمر بصمام الطلب ليوصل هواءً صالحاً ومريحاً للتنفس.</p>
            <p><strong>ملاحظة هامة للتشغيل:</strong> يستهلك الفرد حوالي (40 ليتراً) في الدقيقة، والوقت الاحتياطي للأمان بعد بدء صافرة التحذير هو (10 دقائق) فقط.</p>
            <div class="media-box">
                <div class="video-title">📺 فيديو فني: طريقة فحص وارتداء جهاز التنفس بالهواء المضغوط بشكل صحيح</div>
                <div class="video-container">
                    <iframe src="https://youtube.com" allowfullscreen></iframe>
                </div>
            </div>
        </div>
    </div>

    <!-- الجزء الثاني -->
    <div class="part-group">
        <div class="part-title">الجزء الثاني: الإطفاء</div>

        <!-- الوحدة الخامسة -->
        <div class="section-card">
            <h3>الوحدة الخامسة: الطفايات اليدوية <span class="unit-badge">الوحدة 5</span></h3>
            <p>تُعد الخط الأول لمكافحة الحرائق الصغيرة في بدايتها. تختلف الطفايات بناءً على المادة الإطفائية ورمزها:</p>
            <ul>
                <li><strong>طفاية الماء (الرمز: مثلث أخضر):</strong> تُستخدم للمواد الصلبة ومبدأ عملها هو <strong>التبريد</strong> (ملاحظة: موصلة للكهرباء).</li>
