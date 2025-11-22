<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>شرح رسالة الإمام البربهاري رحمه الله - 10 مجالس</title>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
    <style>
        :root {--main:#1e3a2f;--sec:#2d6a4f;--light:#e8f4f0;--gold:#d4af37;}
        *{box-sizing:border-box;margin:0;padding:0;}
        body{font-family:'Amiri',serif;background:#f5f7f8;color:#2c3e50;line-height:1.9;display:flex;min-height:100vh;flex-direction:column;transition:all 0.4s;}
        .sidebar{width:300px;background:var(--main);color:white;padding:30px 20px;position:fixed;right:0;top:0;bottom:0;overflow-y:auto;box-shadow:-10px 0 25px rgba(0,0,0,0.2);z-index:999;transition:right 0.4s;}
        .sidebar h3{font-size:2rem;text-align:center;margin-bottom:30px;color:var(--gold);border-bottom:3px solid var(--gold);padding-bottom:10px;}
        .sidebar ul{list-style:none;}
        .sidebar a{display:block;padding:18px 22px;background:rgba(255,255,255,0.1);border-radius:12px;margin:10px 0;color:white;font-size:1.4rem;text-decoration:none;transition:0.4s;border-right:6px solid transparent;}
        .sidebar a:hover,.sidebar a.active{background:var(--sec);border-right-color:var(--gold);transform:translateX(-10px);}
        .main-content{flex:1;margin-right:300px;padding:40px;background:white;transition:margin-right 0.4s;position:relative;}
        header{background:linear-gradient(135deg,var(--main),var(--sec));color:white;text-align:center;padding:70px 20px;}
        header h1{font-size:2.8rem;}
        .container{max-width:1150px;margin:0 auto;}
        .tabs{display:flex;flex-wrap:wrap;justify-content:center;gap:12px;margin:40px 0;}
        .tab-btn{background:var(--sec);color:white;padding:14px 28px;border:none;border-radius:50px;cursor:pointer;font-size:1.2rem;transition:0.3s;}
        .tab-btn.active,.tab-btn:hover{background:var(--main);transform:translateY(-4px);}
        .tab-content{display:none;animation:fadeIn 0.6s;}
        .tab-content.active{display:block;}
        details{margin-bottom:16px;border-radius:14px;overflow:hidden;box-shadow:0 4px 15px rgba(0,0,0,0.08);}
        summary{background:var(--sec);color:white;padding:20px;cursor:pointer;font-weight:bold;font-size:1.4rem;list-style:none;display:flex;justify-content:space-between;align-items:center;}
        summary::after{content:"\f077";font-family:"Font Awesome 6 Free";font-weight:900;transition:0.3s;}
        details[open] summary::after{transform:rotate(180deg);}
        .acc-body{padding:30px;background:white;border:2px solid var(--sec);border-top:none;border-radius:0 0 14px 14px;}
        .answer{background:var(--light);padding:25px;border-radius:14px;border-right:6px solid var(--sec);font-size:1.35rem;}
        .correct{color:var(--main);font-weight:bold;}
        .menu-toggle{display:none;position:fixed;top:15px;right:15px;background:var(--main);color:white;width:50px;height:50px;border-radius:50%;font-size:1.5rem;cursor:pointer;z-index:1000;box-shadow:0 4px 15px rgba(0,0,0,0.3);display:flex;align-items:center;justify-content:center;}
        footer{text-align:center;padding:30px;background:var(--main);color:white;margin-top:auto;}

        @keyframes fadeIn{from{opacity:0;}to{opacity:1;}}

        /* تحسينات الجوال - مثالية 100% */
        @media(max-width:992px){
            .sidebar{position:fixed;top:0;right:-300px;width:300px;height:100%;transition:right 0.4s;z-index:999;}
            .sidebar.open{right:0;}
            .main-content{margin-right:0;padding:20px;}
            .menu-toggle{display:flex;}
            header{padding:50px 20px;}
            header h1{font-size:2.2rem;}

            .tabs{flex-direction:column;padding:0 15px;gap:12px;align-items:stretch;}
            .tab-btn{font-size:1.18rem !important;padding:18px 20px !important;border-radius:14px !important;margin:0;}

            details summary{font-size:1.32rem;padding:18px;}
            details summary::after{font-size:1.9rem;min-width:50px;min-height:50px;display:flex;align-items:center;justify-content:center;}
            .acc-body{padding:24px;}
            .answer{font-size:1.28rem;padding:22px;}
        }

        @media(max-width:480px){
            .tab-btn{font-size:1.1rem !important;padding:16px 18px !important;}
            header h1{font-size:2rem;}
        }

        body.sidebar-open{overflow:hidden;}
        .sidebar.open ~ .main-content::before,
        .sidebar.open ~ header::before,
        .sidebar.open ~ footer::before{
            content:"";position:fixed;inset:0;background:rgba(0,0,0,0.55);z-index:998;backdrop-filter:blur(5px);
        }
    </style>
</head>
<body>

<div class="menu-toggle">
    <i class="fas fa-bars"></i>
</div>

<div class="sidebar">
    <h3>مجالس الشرح</h3>
    <ul>
        <li><a href="#" class="active" onclick="showMajlis(1);return false;">المجلس الأول - المقدمة</a></li>
        <li><a href="#" onclick="showMajlis(2);return false;">المجلس الثاني - الشرح الكامل</a></li>
        <li><a href="#" onclick="showMajlis(3);return false;">المجلس الثالث (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(4);return false;">المجلس الرابع (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(5);return false;">المجلس الخامس (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(6);return false;">المجلس السادس (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(7);return false;">المجلس السابع (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(8);return false;">المجلس الثامن (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(9);return false;">المجلس التاسع (قريباً)</a></li>
        <li><a href="#" onclick="showMajlis(10);return false;">المجلس العاشر (قريباً)</a></li>
    </ul>
</div>

<div class="main-content">
    <header>
        <h1>شرح رسالة الإمام البربهاري رحمه الله</h1>
        <p>على عشرة مجالس + 60 سؤال مراجعة شاملة في كل مجلس</p>
    </header>

    <div class="container" id="majlis-content"></div>
</div>

<footer>
    <p>نسأل الله الإخلاص والقبول والثبات على عقيدة السلف الصالح</p>
</footer>

<script>
// ====================== المجلس الأول - كامل 100% ======================
const majlis1 = `
    <div class="tabs">
       <button class="tab-btn active" onclick="openTab(event,'tab1')">معنى العقيدة والاعتقاد</button>
        <button class="tab-btn" onclick="openTab(event,'tab2')">نشأة التصنيف في كتب الاعتقاد</button>
        <button class="tab-btn" onclick="openTab(event,'tab3')">أبرز الكتب العقدية في القرون الأولى</button>
        <button class="tab-btn" onclick="openTab(event,'tab4')">أنواع المصنفات العقدية عند السلف</button>
        <button class="tab-btn" onclick="openTab(event,'tab5')">لماذا نركز على عقيدة السلف دون غيرها؟</button>
        <button class="tab-btn" onclick="openTab(event,'tab6')">60 سؤال مراجعة شاملة</button>
    </div>

    <div id="tab1" class="tab-content active">
        <h2>معنى العقيدة والاعتقاد</h2>
        <details><summary>أصل الكلمة لغة</summary><div class="acc-body">من «عَقَدَ» بمعنى الشد والصلابة → عَقَد العسل إذا اشتدّ، عَقَد النوى إذا صلب</div></details>
        <details><summary>معنى العقيدة اصطلاحاً</summary><div class="acc-body">ما يعقده الإنسان في قلبه عقداً محكماً لا يتزعزع ولا يتزلزل</div></details>
        <details><summary>شدة تمسك أهل الباطل بعقائدهم</summary><div class="acc-body">مشاهد حتى عند أصحاب العقائد الفاسدة → فكيف بأهل العقيدة الصحيحة؟</div></details>
    </div>

    <div id="tab2" class="tab-content">
        <h2>نشأة التصنيف في كتب الاعتقاد</h2>
        <details><summary>متى بدأ التصنيف في السنة عموماً؟</summary><div class="acc-body">في القرن الثاني الهجري</div></details>
        <details><summary>طبيعة التصنيف الأول</summary><div class="acc-body">تصنيف مطلق (مسانيد مرتبة على الرجال لا على الأبواب)</div></details>
        <details><summary>متى بدأ التخصص في مسائل الاعتقاد؟</summary><div class="acc-body">في القرن الثالث الهجري</div></details>
        <details><summary>سمات الكتب العقدية الأولى</summary><div class="acc-body">
            <ul>
                <li>بسيطة وموجزة</li>
                <li>لا تشمل كل مسائل الاعتقاد</li>
                <li>إسنادية غالباً</li>
                <li>لا مناقشات طويلة</li>
            </ul>
        </div></details>
    </div>

    <div id="tab3" class="tab-content">
        <h2>أبرز الكتب العقدية في القرون الأولى</h2>
        <details><summary>الإمام الشافعي (ت 204هـ)</summary><div class="acc-body">اعتقاد الشافعي → ركز على إثبات الأسماء والصفات فقط</div></details>
        <details><summary>ابن أبي شيبة (ت 235هـ)</summary><div class="acc-body">كتاب الإيمان → قضيتان فقط: مسائل الإيمان + حكم تارك الصلاة</div></details>
        <details><summary>الإمام أحمد (مجموع عنه)</summary><div class="acc-body">اعتقاد الإمام أحمد (جمعه التميمي ت 410هـ) → 10 قضايا متنوعة</div></details>
        <details><summary>الإمام البخاري (ت 256هـ)</summary><div class="acc-body">خلق أفعال العباد → محوره القرآن كلام الله غير مخلوق</div></details>
        <details><summary>الإمام المزني (ت 264هـ)</summary><div class="acc-body">شرح السنة → العلو، القدر، القرآن، الصفات، الصراط...</div></details>
        <details><summary>ابن قتيبة (ت 276هـ)</summary><div class="acc-body">الاختلاف في اللفظ والرد على الجهمية والمشبهة</div></details>
        <details><summary>الدارمي (ت 280هـ)</summary><div class="acc-body">الرد على الجهمية</div></details>
        <details><summary>الطبري (ت 310هـ)</summary><div class="acc-body">صريح السنة</div></details>
        <details><summary>الخلال (ت 311هـ)</summary><div class="acc-body">كتاب السنة (موسوعي يخلط الاعتقاد بالأحكام)</div></details>
        <details><summary>ابن أبي داود (ت 316هـ)</summary><div class="acc-body">الحائية في السنة</div></details>
        <details><summary>الإسماعيلي (ت 371هـ) والصابوني (ت 449هـ)</summary><div class="acc-body">اعتقاد الإسماعيلي + عقيدة السلف وأصحاب الحديث</div></details>
    </div>

    <div id="tab4" class="tab-content">
        <h2>أنواع المصنفات العقدية عند أهل السنة</h2>
        <details><summary>كتب موضوعية</summary><div class="acc-body">مثل: كتاب الإيمان، النبوات، الإيمان لابن تيمية (ضخم بحثي)</div></details>
        <details><summary>كتب الشروح</summary><div class="acc-body">شرح الطحاوية، شرح لمعة الاعتقاد، شرح الواسطية...</div></details>
        <details><summary>كتب الردود</summary><div class="acc-body">الرد على الجهمية (أحمد، البخاري، الدارمي)، منهاج السنة (ابن تيمية)، غاية الأماني (الآلوسي)</div></details>
        <details><summary>كتب موسوعية</summary><div class="acc-body">مجموع الفتاوى، الحجة في بيان المحجة (الأصبهاني)</div></details>
    </div>

    <div id="tab5" class="tab-content">
        <h2>لماذا نركز على عقيدة السلف دون منهج المتكلمين؟</h2>
        <details><summary>أبرز عيوب منهج المتكلمين</summary><div class="acc-body">
            <ul>
                <li>معرفة الله بالاستدلال فقط → المقلد توحيده مشكوك فيه</li>
                <li>طغيان الأسلوب الجدلي (فإن قيل... قيل له...)</li>
                <li>مليئة بمصطلحات حادثة (جسم، جوهر، عرض، ملاصقة، استقرار...)</li>
                <li>معقدة، مظلمة، تحتاج مفاتيح كثيرة لفهم جملة واحدة</li>
            </ul>
        </div></details>
        <details><summary>مميزات عقيدة السلف</summary><div class="acc-body">
            <ul>
                <li>مبنية على النص (الكتاب والسنة)</li>
                <li>عقيدة الفطرة والغريزة السليمة</li>
                <li>ربانية → لا تخطئ أبداً</li>
                <li>سهلة يسيرة بلا تكلف ولا تعمق</li>
                <li>واضحة نيرة</li>
                <li>خالية من الاصطلاحات الحادثة</li>
                <li>ترقي صاحبها وتهذب أخلاقه</li>
                <li>تنتج المسلم العقائدي الحامل للرسالة</li>
                <li>تمزج الجنسيات والشعوب تحت راية واحدة</li>
            </ul>
        </div></details>
    </div>

    <div id="tab6" class="tab-content">
        <h2>الأسئلة والمراجعة الشاملة (60 سؤالاً)</h2>
        <p style="text-align:center;font-size:1.5rem;color:var(--sec);margin:35px 0;">اضغط على السؤال لتظهر الإجابة</p>

        <details><summary>1. ما أصل كلمة "العقيدة" لغة؟</summary><div class="acc-body"><div class="answer"><span class="correct">من "عقد": الشد والصلابة (عقد العسل، عقد النوى)</span></div></div></details>
        <details><summary>2. لماذا تكون عقيدة السلف أشد تمسكاً؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأنها حق، وأهل الحق أولى بالحرص</span></div></div></details>
        <details><summary>3. متى بدأ التصنيف في مسائل الاعتقاد؟</summary><div class="acc-body"><div class="answer"><span class="correct">القرن الثالث الهجري</span></div></div></details>
        <details><summary>4. ما طبيعة التصنيف الأول في السنة؟</summary><div class="acc-body"><div class="answer"><span class="correct">تصنيف مطلق (مسانيد على الرجال)</span></div></div></details>
        <details><summary>5. اذكر 4 سمات للكتب العقدية الأولى؟</summary><div class="acc-body"><div class="answer"><span class="correct">بسيطة، موجزة، إسنادية، لا تشمل كل المسائل</span></div></div></details>
        <details><summary>6. أول كتب الاعتقاد المعروفة؟</summary><div class="acc-body"><div class="answer"><span class="correct">اعتقاد الشافعي (ت 204هـ)</span></div></div></details>
        <details><summary>7. محور كتاب الإيمان لابن أبي شيبة؟</summary><div class="acc-body"><div class="answer"><span class="correct">الإيمان + حكم تارك الصلاة</span></div></div></details>
        <details><summary>8. من جمع اعتقاد الإمام أحمد؟</summary><div class="acc-body"><div class="answer"><span class="correct">أبو الفضل التميمي (ت 410هـ)</span></div></div></details>
        <details><summary>9. كم قضية في اعتقاد الإمام أحمد المجموع؟</summary><div class="acc-body"><div class="answer"><span class="correct">10 قضايا</span></div></div></details>
        <details><summary>10. محور "خلق أفعال العباد" للبخاري؟</summary><div class="acc-body"><div class="answer"><span class="correct">القرآن كلام الله غير مخلوق</span></div></div></details>
        <details><summary>11. اسم كتاب الدارمي في الرد على الجهمية؟</summary><div class="acc-body"><div class="answer"><span class="correct">الرد على الجهمية</span></div></div></details>
        <details><summary>12. كتاب الخلال العقدي الموسوعي؟</summary><div class="acc-body"><div class="answer"><span class="correct">كتاب السنة (يخلط الاعتقاد بالأحكام)</span></div></div></details>
        <details><summary>13. القصيدة الحائية لمن؟</summary><div class="acc-body"><div class="answer"><span class="correct">ابن أبي داود (ت 316هـ)</span></div></div></details>
        <details><summary>14. أنواع المصنفات العقدية عند السلف (4 أنواع)؟</summary><div class="acc-body"><div class="answer"><span class="correct">موضوعية، شروح، ردود، موسوعية</span></div></div></details>
        <details><summary>15. مثال على كتب الردود؟</summary><div class="acc-body"><div class="answer"><span class="correct">منهاج السنة، غاية الأماني</span></div></div></details>
        <details><summary>16. أبرز عيوب منهج المتكلمين؟</summary><div class="acc-body"><div class="answer"><span class="correct">الاستدلال فقط، الجدل، المصطلحات الحادثة، التعقيد</span></div></div></details>
        <details><summary>17. أول مميزات عقيدة السلف؟</summary><div class="acc-body"><div class="answer"><span class="correct">مبنية على النص (الكتاب والسنة)</span></div></div></details>
        <details><summary>18. الثانية؟</summary><div class="acc-body"><div class="answer"><span class="correct">عقيدة الفطرة والغريزة السليمة</span></div></div></details>
        <details><summary>19. الثالثة؟</summary><div class="acc-body"><div class="answer"><span class="correct">ربانية → لا تخطئ أبداً</span></div></div></details>
        <details><summary>20. الرابعة؟</summary><div class="acc-body"><div class="answer"><span class="correct">سهلة يسيرة بلا تكلف</span></div></div></details>
        <details><summary>21. الخامسة؟</summary><div class="acc-body"><div class="answer"><span class="correct">واضحة نيرة</span></div></div></details>
        <details><summary>22. السادسة؟</summary><div class="acc-body"><div class="answer"><span class="correct">خالية من الاصطلاحات الحادثة</span></div></div></details>
        <details><summary>23. السابعة؟</summary><div class="acc-body"><div class="answer"><span class="correct">ترقي صاحبها وتهذب أخلاقه</span></div></div></details>
        <details><summary>24. الثامنة؟</summary><div class="acc-body"><div class="answer"><span class="correct">تنتج المسلم العقائدي الحامل للرسالة</span></div></div></details>
        <details><summary>25. التاسعة؟</summary><div class="acc-body"><div class="answer"><span class="correct">تمزج الجنسيات والشعوب تحت راية واحدة</span></div></div></details>
        <details><summary>26. من حمل الدين واللغة بعد العرب غالباً؟</summary><div class="acc-body"><div class="answer"><span class="correct">الأعاجم (البخاري، سيبويه، السلاجقة، المماليك...)</span></div></div></details>
        <details><summary>27. أين بدأ التصنيف في السنة عموماً؟</summary><div class="acc-body"><div class="answer"><span class="correct">القرن الثاني الهجري</span></div></div></details>
        <details><summary>28. مثال على مسند مرتب على الرجال؟</summary><div class="acc-body"><div class="answer"><span class="correct">مسند أحمد، مسند أبي داود الطيالسي</span></div></div></details>
        <details><summary>29. أول كتاب عقدي متخصص معروف؟</summary><div class="acc-body"><div class="answer"><span class="correct">اعتقاد الشافعي</span></div></div></details>
        <details><summary>30. موضوع كتاب "الاختلاف في اللفظ" لابن قتيبة؟</summary><div class="acc-body"><div class="answer"><span class="correct">القدر + الصفات + الرد على الجهمية والمشبهة</span></div></div></details>
        <details><summary>31. كتاب الخلال يخلط ماذا؟</summary><div class="acc-body"><div class="answer"><span class="correct">الاعتقاد بالأحكام ذات الصلة بالاعتقاد</span></div></div></details>
        <details><summary>32. من ألف القصيدة الحائية في السنة؟</summary><div class="acc-body"><div class="answer"><span class="correct">ابن أبي داود</span></div></div></details>
        <details><summary>33. مثال على كتب الشروح؟</summary><div class="acc-body"><div class="answer"><span class="correct">شرح الطحاوية، شرح الواسطية، شرح لمعة الاعتقاد</span></div></div></details>
        <details><summary>34. أشهر كتاب رد على الرافضة؟</summary><div class="acc-body"><div class="answer"><span class="correct">منهاج السنة لابن تيمية</span></div></div></details>
        <details><summary>35. كتاب الآلوسي في الرد على النبهاني؟</summary><div class="acc-body"><div class="answer"><span class="correct">غاية الأماني</span></div></div></details>
        <details><summary>36. أين نجد أوسع الكتب في الاعتقاد؟</summary><div class="acc-body"><div class="answer"><span class="correct">كتب شيخ الإسلام ابن تيمية</span></div></div></details>
        <details><summary>37. أول عيب في منهج المتكلمين؟</summary><div class="acc-body"><div class="answer"><span class="correct">معرفة الله بالاستدلال فقط</span></div></div></details>
        <details><summary>38. ثاني عيب؟</summary><div class="acc-body"><div class="answer"><span class="correct">طغيان الأسلوب الجدلي (فإن قيل... قيل له)</span></div></div></details>
        <details><summary>39. ثالث عيب؟</summary><div class="acc-body"><div class="answer"><span class="correct">مليئة بمصطلحات حادثة (جسم، جوهر، عرض...)</span></div></div></details>
        <details><summary>40. لماذا يحتقر المتضلع في الكلام غيره؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأنه يرى نفسه وصل إلى القمة في المنطق والجدل</span></div></div></details>
        <details><summary>41. عقيدة السلف مبنية على ماذا؟</summary><div class="acc-body"><div class="answer"><span class="correct">النص (الكتاب والسنة)</span></div></div></details>
        <details><summary>42. عقيدة السلف هي عقيدة ماذا؟</summary><div class="acc-body"><div class="answer"><span class="correct">الفطرة والغريزة السليمة</span></div></div></details>
        <details><summary>43. هل تخطئ عقيدة السلف؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا أبداً لأنها ربانية</span></div></div></details>
        <details><summary>44. هل فيها تكلف وتعمق؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، سهلة يسيرة</span></div></div></details>
        <details><summary>45. هل تحتاج مفاتيح لفهم جملها؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، واضحة نيرة</span></div></div></details>
        <details><summary>46. هل فيها اصطلاحات حادثة؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، خالية منها</span></div></div></details>
        <details><summary>47. هل ترقي صاحبها؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم، تهذب أخلاقه وترفعه</span></div></div></details>
        <details><summary>48. هل تنتج جيل المقلدين؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، تنتج المسلم العقائدي الحامل للرسالة</span></div></div></details>
        <details><summary>49. هل تفرق بين الشعوب؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، تمزج الجنسيات تحت راية واحدة</span></div></div></details>
        <details><summary>50. من حفظ اللغة العربية والدين بعد العرب؟</summary><div class="acc-body"><div class="answer"><span class="correct">الأعاجم (سيبويه، البخاري، السلاجقة...)</span></div></div></details>
        <details><summary>51. من أشهر الأعاجم في اللغة؟</summary><div class="acc-body"><div class="answer"><span class="correct">سيبويه، أبو علي الفارسي</span></div></div></details>
        <details><summary>52. من أشهر الأعاجم في الحديث؟</summary><div class="acc-body"><div class="answer"><span class="correct">البخاري، مسلم، الترمذي...</span></div></div></details>
        <details><summary>53. من حمى ديار الإسلام من الدول الأعجمية؟</summary><div class="acc-body"><div class="answer"><span class="correct">السلاجقة، المماليك، العثمانيون</span></div></div></details>
        <details><summary>54. شرف العرب الأول؟</summary><div class="acc-body"><div class="answer"><span class="correct">نقل الدين وحفظه في بدايته</span></div></div></details>
        <details><summary>55. لماذا يجب أن نحافظ على عبارة العالم عند الجمع؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأن تغييرها كذب عليه</span></div></div></details>
        <details><summary>56. الفرق بين التصنيف والجمع؟</summary><div class="acc-body"><div class="answer"><span class="correct">التصنيف تأليف جديد، الجمع تجميع أقوال موجودة</span></div></div></details>
        <details><summary>57. هل كل الكتب العقدية الأولى كتب تأليف أم جمع؟</summary><div class="acc-body"><div class="answer"><span class="correct">كثير منها جمع (مثل اعتقاد الإمام أحمد)</span></div></div></details>
        <details><summary>58. هل يجوز نسبة الكتاب المجموع لصاحبه كاملاً؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم الألفاظ له، لكن الجمع للجامع</span></div></div></details>
        <details><summary>59. لماذا بدأت الكتب العقدية بمسائل محدودة؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأن التصنيف كان في بدايته، والحاجة كانت لمسائل معينة</span></div></div></details>
        <details><summary>60. ما الدعاء الختامي المناسب؟</summary><div class="acc-body"><div class="answer"><span class="correct">اللهم وفقنا لفهم عقيدة السلف والعمل بها والثبات عليها</span></div></div></details>
    </div>
`;

// ====================== المجلس الثاني - كامل 100% ======================
const majlis2 = `
    <div class="tabs">
        <button class="tab-btn active" onclick="openTab(event,'tab2-1')">ترجمة الإمام البربهاري</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-2')">الإسلام هو السنة والسنة هي الإسلام</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-3')">لزوم الجماعة والسواد الأعظم</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-4')">البدعة والمحدثات</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-5')">القاعدة في قبول الأقوال</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-6')">مسائل العقيدة</button>
        <button class="tab-btn" onclick="openTab(event,'tab2-7')">60 سؤال مراجعة</button>
    </div>

    <div id="tab2-1" class="tab-content active">
        <h2>ترجمة الإمام البربهاري رحمه الله</h2>
        <details><summary>اسمه ونسبه</summary><div class="acc-body">الحسن بن علي بن خلف البربهاري (نسبة إلى دواء يجلب من الهند)</div></details>
        <details><summary>مولده ووفاته</summary><div class="acc-body">وُلد سنة 253هـ ≈ وتوفي سنة 329هـ ≈ عاش نحو 76 سنة</div></details>
        <details><summary>شيوخه وتلاميذه</summary><div class="acc-body">صحب تلاميذ الإمام أحمد مباشرة (حنبل بن إسحاق، أبو بكر المروذي…) وعاصَر ابن ماجه وأبا داود صاحبي السنن</div></details>
        <details><summary>أشهر تلاميذه</summary><div class="acc-body">الإمام ابن بطة العكبري صاحب «الإبانة»</div></details>
        <details><summary>شدته على أهل البدع</summary><div class="acc-body">كان قوالاً بالحق لا تأخذه في الله لومة لائم، فأُوشي به إلى الخليفة فهرب واستتر حتى مات مستتراً</div></details>
        <details><summary>قول ابن بطة فيه</summary><div class="acc-body">«إذا رأيت البغدادي يحب أبا الحسن بن بشار وأبا محمد البربهاري فاعلم أنه صاحب سنة»</div></details>
    </div>

    <div id="tab2-2" class="tab-content">
        <h2>الإسلام هو السنة والسنة هي الإسلام</h2>
        <blockquote>اعلموا أن الإسلام هو السنة والسنة هي الإسلام ولا يقوم أحدهما إلا بالآخر</blockquote>
        <details><summary>معنى هذه العبارة</summary><div class="acc-body">الإسلام الذي جاء به محمد ﷺ هو ما كان عليه الصحابة، وهو السنة، فلا ينفك أحدهما عن الآخر</div></details>
    </div>

    <div id="tab2-3" class="tab-content">
        <h2>لزوم الجماعة والسواد الأعظم</h2>
        <details><summary>معنى الجماعة عند السلف</summary><div class="acc-body">ليس المقصود جماعة دعوية أو حزبية، بل من تمسك بالحق ولو كان واحداً</div></details>
        <details><summary>تفسير السواد الأعظم</summary><div class="acc-body">الحق وأهله، حتى لو كانوا قليلاً، كما فسر عبد الرحمن بن زيد بن أسلم بأنه رجل واحد</div></details>
        <details><summary>أبو بكر رضي الله عنه يوم الردة</summary><div class="acc-body">كان هو الجماعة، وانقاد له الصحابة</div></details>
        <details><summary>قول عمر رضي الله عنه</summary><div class="acc-body">لا عذر لأحد في ضلالة ركبها حسبها هدى، ولا في هدى تركه حسبه ضلالة</div></details>
    </div>

    <div id="tab2-4" class="tab-content">
        <h2>البدعة والمحدثات</h2>
        <details><summary>الناس لم يبتدعوا بدعة حتى تركوا من السنة مثلها</summary><div class="acc-body">إذا أحدثت بدعة سُلب منك سنة بقدرها، ولا تعود إليك أبداً</div></details>
        <details><summary>احذر صغار المحدثات</summary><div class="acc-body">كل بدعة كانت أولها صغيرة تشبه الحق، ثم نمت حتى صارت ديناً يُدان به</div></details>
        <details><summary>كيف تبدأ البدع؟</summary><div class="acc-body">تتلبس بالحق وتستدل بالنصوص العامة، كالخوارج بـ «إن الحكم إلا لله»، والديمقراطيون بـ «وأمرهم شورى بينهم»</div></details>
    </div>

    <div id="tab2-5" class="tab-content">
        <h2>القاعدة الذهبية في قبول الأقوال</h2>
        <blockquote>فانظر رحمك الله كل من سمعت كلامه من أهل زمانك خاصة فلا تعجلن ولا تدخلن في شيء منه حتى تسأل وتنظر: هل تكلم به أصحاب رسول الله ﷺ أو أحد من العلماء؟</blockquote>
        <details><summary>معنى القاعدة</summary><div class="acc-body">لا تتبع قولاً إلا إذا وجدت له أثراً عن الصحابة أو العلماء الثقات</div></details>
        <details><summary>كلام العلماء مرتبط بالمناسبة</summary><div class="acc-body">فصل كلام العالم عن مناسبته كذب عليه (مثال فتاوى البرلمان في سياق الجزائر والكويت)</div></details>
    </div>

    <div id="tab2-6" class="tab-content">
        <h2>مسائل العقيدة من الرسالة</h2>
        <details><summary>القرآن كلام الله غير مخلوق</summary><div class="acc-body">والمراء فيه كفر</div></details>
        <details><summary>صفات الله على ظاهرها بلا كيف ولا تعطيل</summary><div class="acc-body">لا يقال «كيف» ولا «لماذا»</div></details>
        <details><summary>الإيمان بالرؤية يوم القيامة</summary><div class="acc-body">يرى المؤمنون ربهم بأبصارهم بلا حجاب ولا ترجمان</div></details>
        <details><summary>الإيمان بالميزان والحوض والصراط والشفاعة وعذاب القبر</summary><div class="acc-body">كلها ثابتة بالكتاب والسنة</div></details>
        <details><summary>الجنة والنار مخلوقتان الآن ولا تفنيان أبداً</summary><div class="acc-body">الجنة فوق السموات السبع، والنار تحت الأرضين السبع</div></details>
        <details><summary>الإيمان بالدجال ونزول عيسى ابن مريم</summary><div class="acc-body">ينزل عيسى فيقتل الدجال</div></details>
    </div>

    <div id="tab2-7" class="tab-content">
        <h2>الأسئلة والمراجعة الشاملة (60 سؤالاً)</h2>
        <p style="text-align:center;font-size:1.5rem;color:var(--sec);margin:35px 0;">اضغط على السؤال لتظهر الإجابة</p>
        <details><summary>1. ما اسم الإمام البربهاري الكامل؟</summary><div class="acc-body"><div class="answer"><span class="correct">الحسن بن علي بن خلف البربهاري</span></div></div></details>
        <details><summary>2. متى وُلد ومتى توفي رحمه الله؟</summary><div class="acc-body"><div class="answer"><span class="correct">253 - 329 هـ</span></div></div></details>
        <details><summary>3. ما معنى "البربهاري" في نسبته؟</summary><div class="acc-body"><div class="answer"><span class="correct">نسبة إلى بيع دواء يُجلب من الهند</span></div></div></details>
        <details><summary>4. من أشهر تلاميذ البربهاري؟</summary><div class="acc-body"><div class="answer"><span class="correct">ابن بطة العكبري صاحب "الإبانة الكبرى"</span></div></div></details>
        <details><summary>5. لماذا مات البربهاري مستتراً؟</summary><div class="acc-body"><div class="answer"><span class="correct">لشدة دعوته للسنة ومواجهته لأهل البدع فأوشي به إلى السلطان</span></div></div></details>
        <details><summary>6. ماذا قال ابن بطة عن محبة البربهاري؟</summary><div class="acc-body"><div class="answer"><span class="correct">إذا رأيت البغدادي يحب أبا محمد البربهاري فاعلم أنه صاحب سنة</span></div></div></details>
        <details><summary>7. ما أصل قوله: الإسلام هو السنة والسنة هي الإسلام؟</summary><div class="acc-body"><div class="answer"><span class="correct">كلام الإمام البربهاري رحمه الله</span></div></div></details>
        <details><summary>8. هل يقوم أحدهما بدون الآخر؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا</span></div></div></details>
        <details><summary>9. ما المقصود بلزوم الجماعة عند السلف؟</summary><div class="acc-body"><div class="answer"><span class="correct">ليس جماعة دعوية، بل من تمسك بالحق ولو كان واحداً</span></div></div></details>
        <details><summary>10. من هو السواد الأعظم؟</summary><div class="acc-body"><div class="answer"><span class="correct">الحق وأهله ولو قلّوا</span></div></div></details>
        <details><summary>11. اذكر مثالاً على الجماعة وهي شخص واحد؟</summary><div class="acc-body"><div class="answer"><span class="correct">أبو بكر الصديق يوم قتال المرتدين</span></div></div></details>
        <details><summary>12. قول عمر: لا عذر لأحد في ضلالة... أكمله؟</summary><div class="acc-body"><div class="answer"><span class="correct">ركبها حسبها هدى، ولا في هدى تركه حسبه ضلالة</span></div></div></details>
        <details><summary>13. هل يُقاس الدين بعقول الرجال؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، بل يُقاس الرجال بالدين</span></div></div></details>
        <details><summary>14. من خالف الصحابة في شيء من أمر الدين ماذا يكون؟</summary><div class="acc-body"><div class="answer"><span class="correct">كافر (حسب نوع المخالفة)</span></div></div></details>
        <details><summary>15. الناس لم يبتدعوا بدعة إلا بعد ماذا؟</summary><div class="acc-body"><div class="answer"><span class="correct">تركوا من السنة مثلها</span></div></div></details>
        <details><summary>16. هل تعود السنة بعد تركها لأجل بدعة؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا تعود أبداً</span></div></div></details>
        <details><summary>17. كل بدعة كانت أولها صغيرة تشبه ماذا؟</summary><div class="acc-body"><div class="answer"><span class="correct">الحق</span></div></div></details>
        <details><summary>18. كيف تبدأ البدع غالباً؟</summary><div class="acc-body"><div class="answer"><span class="correct">تتلبس بالحق وتستدل بالنصوص العامة</span></div></div></details>
        <details><summary>19. اذكر مثالاً تاريخياً على بدعة تلبست بالحق؟</summary><div class="acc-body"><div class="answer"><span class="correct">الخوارج بـ «إن الحكم إلا لله»</span></div></div></details>
        <details><summary>20. القاعدة الذهبية في قبول الأقوال؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا تعجل حتى تسأل: هل تكلم به الصحابة أو العلماء الثقات؟</span></div></div></details>
        <details><summary>21. فصل كلام العالم عن مناسبته = ؟</summary><div class="acc-body"><div class="answer"><span class="correct">كذب عليه</span></div></div></details>
        <details><summary>22. من زعم أن الصحابة لم يكفوا أمر الإسلام فقد...؟</summary><div class="acc-body"><div class="answer"><span class="correct">كذبهم وهو مبتدع ضال مضل</span></div></div></details>
        <details><summary>23. هل في السنة قياس مذموم؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا</span></div></div></details>
        <details><summary>24. حكم الجدال والمراء في الدين؟</summary><div class="acc-body"><div class="answer"><span class="correct">محدث يقدح الشك في القلب</span></div></div></details>
        <details><summary>25. حكم الكلام في الرب بغير ما وصف به نفسه؟</summary><div class="acc-body"><div class="answer"><span class="correct">بدعة وضلالة</span></div></div></details>
        <details><summary>26. هل نقول في صفات الله "كيف" أو "لماذا"؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا</span></div></div></details>
        <details><summary>27. حكم القرآن؟</summary><div class="acc-body"><div class="answer"><span class="correct">كلام الله غير مخلوق، والمراء فيه كفر</span></div></div></details>
        <details><summary>28. هل يرى المؤمنون ربهم يوم القيامة؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم، بأبصارهم بلا حجاب ولا ترجمان</span></div></div></details>
        <details><summary>29. ما حكم الميزان يوم القيامة؟</summary><div class="acc-body"><div class="answer"><span class="correct">ثابت له كفتان ولسان</span></div></div></details>
        <details><summary>30. ما حكم عذاب القبر ومنكر ونكير؟</summary><div class="acc-body"><div class="answer"><span class="correct">حق</span></div></div></details>
        <details><summary>31. هل لرسول الله حوض؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم، ثابت بالسنة الصحيحة</span></div></div></details>
        <details><summary>32. من له الشفاعة العظمى؟</summary><div class="acc-body"><div class="answer"><span class="correct">محمد صلى الله عليه وسلم</span></div></div></details>
        <details><summary>33. لمن تكون شفاعة النبي يوم القيامة؟</summary><div class="acc-body"><div class="answer"><span class="correct">للمذنبين الخاطئين من أمته</span></div></div></details>
        <details><summary>34. هل يخرج أحد من النار بعد دخولها؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم بشفاعة النبي والصالحين ثم تفضل الله</span></div></div></details>
        <details><summary>35. صف الصراط؟</summary><div class="acc-body"><div class="answer"><span class="correct">أدق من الشعرة وأحد من السيف، مضروب على متن جهنم</span></div></div></details>
        <details><summary>36. هل الجنة والنار مخلوقتان الآن؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم</span></div></div></details>
        <details><summary>37. هل تفنيان أبداً؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، باقيتان أبد الآبدين</span></div></div></details>
        <details><summary>38. أين الجنة والنار؟</summary><div class="acc-body"><div class="answer"><span class="correct">الجنة فوق السموات السبع وسقفها العرش، والنار تحت الأرضين السبع</span></div></div></details>
        <details><summary>39. هل الجنة التي كان فيها آدم هي جنة الخلد؟</summary><div class="acc-body"><div class="answer"><span class="correct">فيها خلاف كبير بين العلماء</span></div></div></details>
        <details><summary>40. هل يؤمن أهل السنة بالمسيح الدجال؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم</span></div></div></details>
        <details><summary>41. من يقتل الدجال؟</summary><div class="acc-body"><div class="answer"><span class="correct">عيسى بن مريم عليه السلام</span></div></div></details>
        <details><summary>42. ما معنى مجالسة المناصحة؟</summary><div class="acc-body"><div class="answer"><span class="correct">تفتح باب الفائدة</span></div></div></details>
        <details><summary>43. ما معنى مجالسة المناظرة؟</summary><div class="acc-body"><div class="answer"><span class="correct">تغلق باب الفائدة</span></div></div></details>
        <details><summary>44. لماذا كان تناظر السلف للمناصحة وليس للمغالبه؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأنهم يريدون الحق، بخلاف أهل البدع</span></div></div></details>
        <details><summary>45. هل كل مخالفة للصحابة كفر؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، بل بحسب نوع المخالفة (كفر، بدعة، معصية)</span></div></div></details>
        <details><summary>46. لماذا سمي العيد عيداً؟</summary><div class="acc-body"><div class="answer"><span class="correct">لأنه يعود (يذهب ويجيء)</span></div></div></details>
        <details><summary>47. ما الفرق بين الزلة والعناد؟</summary><div class="acc-body"><div class="answer"><span class="correct">الزلة: من زل وهو يريد الخير، والعناد: من عاند الحق</span></div></div></details>
        <details><summary>48. من يجب تحذير الناس منه؟</summary><div class="acc-body"><div class="answer"><span class="correct">العاند الضال المضل</span></div></div></details>
        <details><summary>49. هل يجوز الجدال في الصفات؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، بل نؤمن بها كما جاءت بلا كيف</span></div></div></details>
        <details><summary>50. هل يقال في الله "متى" أو "أين" بمعنى الحدود؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا، هو الأول بلا متى والآخر بلا منتهى</span></div></div></details>
        <details><summary>51. هل علم الله محيط بكل شيء؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم، لا يخلو من علمه مكان</span></div></div></details>
        <details><summary>52. هل الإيمان بالقدر من السنة؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم</span></div></div></details>
        <details><summary>53. هل يجوز ضرب الأمثال لله؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا</span></div></div></details>
        <details><summary>54. هل الشفاعة تشمل المشركين؟</summary><div class="acc-body"><div class="answer"><span class="correct">لا</span></div></div></details>
        <details><summary>55. هل يخرج من النار من قال لا إله إلا الله؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم بشفاعة أو تفضل الله</span></div></div></details>
        <details><summary>56. هل النور على الصراط على قدر الإيمان؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم</span></div></div></details>
        <details><summary>57. هل يؤمن أهل السنة بالملائكة؟</summary><div class="acc-body"><div class="answer"><span class="correct">نعم</span></div></div></details>
        <details><summary>58. من ينزل لقتل الدجال؟</summary><div class="acc-body"><div class="answer"><span class="correct">عيسى بن مريم عليه السلام</span></div></div></details>
        <details><summary>59. هل كل نبي له حوض؟</summary><div class="acc-body"><div class="answer"><span class="correct">فيه آثار، لكن حوض محمد ﷺ ثابت قطعاً</span></div></div></details>
        <details><summary>60. ما الدعاء الختامي المناسب لهذه الرسالة؟</summary><div class="acc-body"><div class="answer"><span class="correct">اللهم ثباتنا على السنة حتى نلقاك</span></div></div></details>
    </div>
`;

// تحميل المجلس الأول عند فتح الصفحة
document.getElementById('majlis-content').innerHTML = majlis1;

// وظائف التنقل والتبويبات
function showMajlis(num) {
    document.querySelectorAll('.sidebar a').forEach(a => a.classList.remove('active'));
    event.target.classList.add('active');
    if (num == 1) document.getElementById('majlis-content').innerHTML = majlis1;
    else if (num == 2) document.getElementById('majlis-content').innerHTML = majlis2;
    else {
        document.getElementById('majlis-content').innerHTML = `<h2 style="text-align:center;padding:120px 20px;font-size:2rem;color:var(--sec);">المجلس ${num} - قريباً إن شاء الله</h2>`;
    }
    if(window.innerWidth <= 992){
        document.querySelector('.sidebar').classList.remove('open');
        document.body.classList.remove('sidebar-open');
    }
}

function openTab(evt, tabName) {
    document.querySelectorAll(".tab-content").forEach(t => t.classList.remove("active"));
    document.querySelectorAll(".tab-btn").forEach(b => b.classList.remove("active"));
    document.getElementById(tabName).classList.add("active");
    evt.currentTarget.classList.add("active");
    if(window.innerWidth <= 992){
        window.scrollTo({top: document.querySelector('header').offsetHeight + 70, behavior: 'smooth'});
    }
}

// فتح وإغلاق الـ Sidebar
document.querySelector('.menu-toggle').addEventListener('click', function(e) {
    e.stopPropagation();
    document.querySelector('.sidebar').classList.toggle('open');
    document.body.classList.toggle('sidebar-open');
});

// إغلاق الـ Sidebar بالضغط خارجها
document.addEventListener('click', function(e) {
    if (window.innerWidth <= 992) {
        const sidebar = document.querySelector('.sidebar');
        const toggle = document.querySelector('.menu-toggle');
        if (sidebar.classList.contains('open') && !sidebar.contains(e.target) && !toggle.contains(e.target)) {
            sidebar.classList.remove('open');
            document.body.classList.remove('sidebar-open');
        }
    }
});
</script>
</body>
</html>
