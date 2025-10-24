 <!DOCTYPE html>

<html dir="rtl" lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HSE - HADID CHEMAL</title>
    <style>
        /* =================== CSS - التصميم =================== */

```
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: #f5f7fa;
        color: #333;
    }
    
    /* ===== رأس الصفحة (Header) ===== */
    .header {
        background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
        color: white;
        padding: 40px 20px;
        text-align: center;
        box-shadow: 0 4px 15px rgba(0,0,0,0.2);
    }
    
    .header h1 {
        font-size: 42px;
        margin-bottom: 10px;
        letter-spacing: 2px;
        text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    }
    
    .header p {
        font-size: 18px;
        opacity: 0.95;
    }
    
    /* ===== الحاوية الرئيسية ===== */
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 30px 20px;
    }
    
    /* ===== قسم الطوارئ (مميز بالأحمر) ===== */
    .emergency-section {
        background: linear-gradient(135deg, #c0392b 0%, #e74c3c 100%);
        color: white;
        padding: 30px;
        border-radius: 15px;
        margin-bottom: 30px;
        box-shadow: 0 8px 25px rgba(231, 76, 60, 0.3);
        animation: pulse 2s infinite;
    }
    
    @keyframes pulse {
        0%, 100% { transform: scale(1); }
        50% { transform: scale(1.02); }
    }
    
    .emergency-section h2 {
        font-size: 28px;
        margin-bottom: 20px;
        text-align: center;
        border-bottom: 2px solid white;
        padding-bottom: 15px;
    }
    
    .emergency-section .warning-icon {
        text-align: center;
        font-size: 60px;
        margin-bottom: 20px;
    }
    
    .phone-numbers {
        display: flex;
        gap: 15px;
        justify-content: center;
        flex-wrap: wrap;
        margin-top: 20px;
    }
    
    .phone-btn {
        background: white;
        color: #e74c3c;
        padding: 15px 30px;
        border-radius: 50px;
        text-decoration: none;
        font-size: 20px;
        font-weight: bold;
        box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        transition: all 0.3s;
        display: flex;
        align-items: center;
        gap: 10px;
    }
    
    .phone-btn:hover {
        transform: translateY(-3px);
        box-shadow: 0 6px 20px rgba(0,0,0,0.3);
        background: #f8f9fa;
    }
    
    /* ===== البطاقات (Cards) ===== */
    .cards-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 25px;
        margin-top: 30px;
    }
    
    .card {
        background: white;
        padding: 30px;
        border-radius: 15px;
        box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        transition: all 0.3s;
        border-right: 5px solid #2a5298;
    }
    
    .card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 30px rgba(0,0,0,0.15);
    }
    
    .card-icon {
        font-size: 50px;
        text-align: center;
        margin-bottom: 20px;
    }
    
    .card h3 {
        color: #1e3c72;
        font-size: 22px;
        margin-bottom: 15px;
        text-align: center;
        border-bottom: 2px solid #2a5298;
        padding-bottom: 10px;
    }
    
    .card p {
        color: #555;
        line-height: 1.8;
        font-size: 16px;
    }
    
    .card ul {
        margin-right: 20px;
        margin-top: 15px;
    }
    
    .card li {
        margin-bottom: 10px;
        color: #555;
        line-height: 1.6;
    }
    
    /* ===== زر واتساب ===== */
    .whatsapp-btn {
        background: #25D366;
        color: white;
        padding: 12px 25px;
        border-radius: 25px;
        text-decoration: none;
        display: inline-flex;
        align-items: center;
        gap: 10px;
        margin-top: 15px;
        font-weight: bold;
        transition: all 0.3s;
        box-shadow: 0 4px 15px rgba(37, 211, 102, 0.3);
    }
    
    .whatsapp-btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
        background: #20BA5A;
    }
    
    /* ===== زر الاتصال بالمكتب ===== */
    .contact-office-btn {
        background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
        color: white;
        padding: 12px 25px;
        border-radius: 25px;
        text-decoration: none;
        display: inline-block;
        margin-top: 15px;
        font-weight: bold;
        transition: all 0.3s;
        box-shadow: 0 4px 15px rgba(42, 82, 152, 0.3);
    }
    
    .contact-office-btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 6px 20px rgba(42, 82, 152, 0.4);
    }
    
    /* ===== التذييل (Footer) ===== */
    .footer {
        background: #1e3c72;
        color: white;
        text-align: center;
        padding: 25px;
        margin-top: 50px;
    }
    
    .footer p {
        opacity: 0.9;
    }
    
    /* ===== التجاوب مع الموبايل ===== */
    @media (max-width: 768px) {
        .header h1 {
            font-size: 28px;
        }
        
        .phone-numbers {
            flex-direction: column;
        }
        
        .phone-btn {
            width: 100%;
            justify-content: center;
        }
    }
</style>
```

</head>
<body>

```
<!-- =================== HTML - الهيكل =================== -->

<!-- رأس الصفحة -->
<div class="header">
    <h1>HSE - HADID CHEMAL</h1>
    <p>مكتب الصحة والسلامة المهنية</p>
</div>

<!-- المحتوى الرئيسي -->
<div class="container">
    
    <!-- قسم الطوارئ -->
    <div class="emergency-section">
        <div class="warning-icon">⚠️</div>
        <h2>أرقام الطوارئ</h2>
        <p style="text-align: center; font-size: 18px; margin-bottom: 20px;">
            في حال وجود حادث أو أي شيء قد يشكل خطراً<br>
            يرجى الاتصال بالمكتب فوراً على الأرقام التالية:
        </p>
        
        <div class="phone-numbers">
            <a href="tel:38889163" class="phone-btn">
                📞 38889163
            </a>
            <a href="tel:38889169" class="phone-btn">
                📞 38889169
            </a>
            <a href="tel:43088081" class="phone-btn">
                📞 43088081
            </a>
            <a href="tel:33332423" class="phone-btn">
                📞 33332423
            </a>
        </div>
    </div>
    
    <!-- البطاقات -->
    <div class="cards-container">
        
        <!-- بطاقة النظافة -->
        <div class="card">
            <div class="card-icon">🧹</div>
            <h3>النظافة والسلامة</h3>
            <p>
                يجب الحفاظ على نظافة جميع أرجاء الشركة لضمان بيئة عمل آمنة وصحية للجميع.
            </p>
            <p style="margin-top: 15px; font-weight: bold; color: #2a5298;">
                النظافة مسؤولية الجميع ✨
            </p>
            <p style="margin-top: 20px; font-weight: bold; color: #333;">
                يرجى إبلاغ المكتب:
            </p>
            <a href="https://wa.me/43088081?text=مرحباً، أريد الإبلاغ عن موضوع النظافة" class="whatsapp-btn" target="_blank">
                💬 تواصل عبر واتساب
            </a>
        </div>
        
        <!-- بطاقة طفايات الحريق -->
        <div class="card">
            <div class="card-icon">🧯</div>
            <h3>طفايات الحريق</h3>
            <p>
                في حال رأيت أي واحدة من طفايات الحريق في حالة غير سليمة، يرجى إبلاغ المكتب فوراً.
            </p>
            <p style="margin-top: 15px;">
                <strong>ملاحظة:</strong> تفقد الطفايات بشكل دوري للتأكد من سلامتها.
            </p>
            <p style="margin-top: 20px; font-weight: bold; color: #333;">
                يرجى إبلاغ المكتب:
            </p>
            <a href="https://wa.me/43088081?text=مرحباً، أريد الإبلاغ عن طفاية حريق بحاجة للصيانة" class="whatsapp-btn" target="_blank">
                💬 تواصل عبر واتساب
            </a>
        </div>
        
        <!-- بطاقة معدات الحماية -->
        <div class="card">
            <div class="card-icon">🦺</div>
            <h3>معدات الحماية الشخصية (EPI)</h3>
            <p>
                في حال حان وقت استلام أي عامل لمعدات الحماية الشخصية (EPI)، يرجى التوجه إلى المكتب.
            </p>
            <ul>
                <li>خوذة السلامة</li>
                <li>نظارات الحماية</li>
                <li>القفازات</li>
                <li>الأحذية الواقية</li>
                <li>السترات العاكسة</li>
            </ul>
            <p style="margin-top: 20px; font-weight: bold; color: #333;">
                يرجى إبلاغ المكتب:
            </p>
            <a href="https://wa.me/43088081?text=مرحباً، أريد استلام معدات الحماية الشخصية EPI" class="whatsapp-btn" target="_blank">
                💬 تواصل عبر واتساب
            </a>
        </div>
        
    </div>
    
</div>

<!-- التذييل -->
<div class="footer">
    <p><strong>HSE - HADID CHEMAL</strong></p>
    <p>مكتب الصحة والسلامة المهنية</p>
    <p style="margin-top: 10px; opacity: 0.8;">السلامة أولاً 🛡️</p>
</div>

<!-- =================== JavaScript - التفاعل =================== -->
<script>
    // رسالة ترحيب في console
    console.log('🛡️ مرحباً بك في موقع HSE - HADID CHEMAL');
</script>
```

</body>
</html>