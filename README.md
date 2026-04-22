
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes, viewport-fit=cover">
    <title>Карьерный навигатор | Инженер цифровых мостов | Сетевой администратор</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', 'Roboto', system-ui, -apple-system, sans-serif;
            background: linear-gradient(145deg, #0a2f3a 0%, #0a4b5e 100%);
            min-height: 100vh;
            padding: 16px 12px 40px;
        }

        .container {
            max-width: 650px;
            margin: 0 auto;
        }

        .card {
            background: rgba(255,255,255,0.97);
            border-radius: 32px;
            padding: 24px 18px;
            margin-bottom: 20px;
            box-shadow: 0 15px 30px -10px rgba(0,0,0,0.3);
        }

        h1 {
            font-size: 1.6rem;
            font-weight: 800;
            background: linear-gradient(135deg, #FFE6B0, #FFB347);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 8px;
            line-height: 1.3;
        }

        .subhead {
            font-size: 0.9rem;
            color: #2c5368;
            margin-bottom: 20px;
            line-height: 1.4;
        }

        .info-block {
            background: #eef2fa;
            border-radius: 24px;
            padding: 18px;
            margin-bottom: 24px;
            border-left: 5px solid #FFB347;
        }

        .info-title {
            font-weight: 800;
            font-size: 1rem;
            margin-bottom: 12px;
            color: #1e4a6e;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .info-text {
            font-size: 0.9rem;
            line-height: 1.45;
            color: #1e3a4a;
            margin-bottom: 12px;
        }

        .salary-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-top: 12px;
        }

        .salary-item {
            background: white;
            border-radius: 40px;
            padding: 8px 16px;
            flex: 1;
            text-align: center;
            box-shadow: 0 2px 6px rgba(0,0,0,0.05);
        }

        .salary-value {
            font-weight: 800;
            font-size: 1.2rem;
            color: #1e6f5c;
        }

        .salary-label {
            font-size: 0.7rem;
            color: #5a6e7a;
        }

        h2 {
            font-size: 1.3rem;
            font-weight: 700;
            color: #1e4a6e;
            margin-bottom: 16px;
            display: flex;
            align-items: center;
            gap: 8px;
            flex-wrap: wrap;
        }

        .badge {
            background: #FFB347;
            color: #1e3a4a;
            padding: 4px 12px;
            border-radius: 40px;
            font-size: 0.7rem;
            font-weight: 600;
        }

        .category-btns {
            display: flex;
            gap: 10px;
            margin-bottom: 28px;
            flex-wrap: wrap;
        }

        .cat-btn {
            flex: 1;
            background: #eef2f5;
            border: none;
            padding: 14px 8px;
            border-radius: 60px;
            font-weight: 700;
            font-size: 1rem;
            cursor: pointer;
            transition: 0.2s;
            color: #1e4a6e;
            text-align: center;
        }

        .cat-btn.active {
            background: #FFB347;
            color: #1e3a4a;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        .question {
            margin: 20px 0 20px;
            transition: all 0.3s ease;
            background: #ffffff;
            border-radius: 28px;
            padding: 8px;
        }

        .question-highlight {
            animation: highlightBorder 0.5s ease;
            background: #fff8f0;
            box-shadow: 0 0 0 3px #FFB347;
        }

        @keyframes highlightBorder {
            0% { box-shadow: 0 0 0 0 #FFB347; background: #fff1e0; }
            50% { box-shadow: 0 0 0 8px #FFB34780; background: #fff1e0; }
            100% { box-shadow: 0 0 0 3px #FFB347; background: #fff8f0; }
        }

        .question p {
            font-weight: 700;
            margin-bottom: 16px;
            font-size: 1.1rem;
            color: #1e3a4a;
            background: #fff1e0;
            padding: 12px 16px;
            border-radius: 28px;
        }

        .option-row {
            display: flex;
            flex-direction: column;
            gap: 12px;
            margin-bottom: 12px;
        }

        .option-btn {
            background: #f0f5fa;
            padding: 14px 18px;
            border-radius: 60px;
            border: 1px solid #cbdbe0;
            cursor: pointer;
            transition: 0.1s;
            font-size: 1rem;
            font-weight: 500;
            text-align: center;
            color: #1e4a6e;
        }

        .option-btn.selected {
            background: #1e6f5c;
            border-color: #1e6f5c;
            color: white;
        }

        .next-btn {
            background: #FFB347;
            border: none;
            width: 100%;
            padding: 16px;
            border-radius: 60px;
            font-weight: bold;
            font-size: 1.1rem;
            margin-top: 20px;
            cursor: pointer;
            color: #1e3a4a;
        }

        .map-grid {
            display: flex;
            flex-direction: column;
            gap: 16px;
            margin: 20px 0;
        }

        .map-stage {
            background: white;
            border-radius: 28px;
            padding: 16px 18px;
            border-left: 8px solid #FFB347;
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);
            transition: 0.2s;
        }

        .stage-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            margin-bottom: 10px;
            gap: 8px;
        }

        .stage-number {
            background: #FFB347;
            width: 40px;
            height: 40px;
            border-radius: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 800;
            font-size: 1.2rem;
            color: #1e3a4a;
        }

        .stage-title {
            font-size: 1.1rem;
            font-weight: 700;
            color: #1e4a6e;
            flex: 1;
        }

        .stage-desc {
            color: #2c5368;
            margin: 10px 0;
            font-size: 0.9rem;
            line-height: 1.45;
        }

        .links {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 12px;
        }

        .link-btn {
            background: #eef2f5;
            padding: 8px 14px;
            border-radius: 40px;
            font-size: 0.75rem;
            text-decoration: none;
            color: #1e6f5c;
            font-weight: 600;
            display: inline-block;
            word-break: break-word;
        }

        .back-btn {
            background: #1e6f5c;
            color: white;
            border: none;
            padding: 14px 20px;
            border-radius: 60px;
            font-weight: 600;
            margin-bottom: 16px;
            width: 100%;
            font-size: 1rem;
        }

        .footer-note {
            font-size: 0.7rem;
            text-align: center;
            margin-top: 24px;
            color: rgba(255,255,240,0.8);
            line-height: 1.4;
        }

        .hidden {
            display: none;
        }

        .recommend-block {
            background: #fff1e0;
            border-radius: 28px;
            padding: 18px;
            margin-bottom: 20px;
        }

        .recommend-label {
            font-size: 0.85rem;
            font-weight: 600;
            color: #1e6f5c;
        }

        .recommend-stage-name {
            font-weight: 800;
            font-size: 1.2rem;
            color: #1e6f5c;
            margin: 6px 0 8px;
        }

        .recommend-text {
            font-size: 0.9rem;
            line-height: 1.4;
            color: #2c5368;
        }

        @media (max-width: 480px) {
            body { padding: 12px 10px 30px; }
            .card { padding: 20px 14px; }
            h1 { font-size: 1.4rem; }
            .info-block { padding: 14px; }
            .salary-item { padding: 6px 12px; }
            .salary-value { font-size: 1rem; }
            .cat-btn { padding: 12px 6px; font-size: 0.9rem; }
            .question p { font-size: 1rem; padding: 10px 14px; }
            .option-btn { padding: 12px 14px; font-size: 0.9rem; }
            .stage-title { font-size: 1rem; }
        }
    </style>
</head>
<body>
<div class="container" id="app">
    <!-- СТРАНИЦА 1: ОПРОС + ИНФОРМАЦИОННАЯ СПРАВКА -->
    <div id="pageSurvey">
        <div class="card">
            <h1>🌉 Карьерный навигатор</h1>
            <div class="subhead">Инженер цифровых мостов — сетевой и системный администратор для космодрома, ГПЗ, мостов, канатной дороги, ГЭС.</div>

            <!-- ИНФОРМАЦИОННАЯ СПРАВКА -->
            <div class="info-block">
                <div class="info-title"><span>🖧</span> Кто такой сетевой и системный администратор?</div>
                <div class="info-text">
                    Это специалист, который проектирует, настраивает и защищает компьютерные сети, серверы и IT-инфраструктуру. Он — «строитель цифровых мостов», без которого не работают ни заводы, ни космодромы. В Амурской области такие специалисты обеспечивают связанность стратегических объектов: <strong>космодрома Восточный, ГПЗ, международных мостов, канатной дороги и ГЭС</strong>.
                </div>
                <div class="info-title"><span>📊</span> Востребованность в России и Амурской области</div>
                <div class="info-text">
                    • В России ежегодно требуется более <strong>50 000 IT-специалистов</strong>.<br>
                    • В Амурской области только в 2026 году открыто <strong>более 200 вакансий</strong>.<br>
                    • Профессия входит в ТОП-10 самых востребованных.
                </div>
                <div class="info-title"><span>💰</span> Средние зарплаты</div>
                <div class="salary-grid">
                    <div class="salary-item"><div class="salary-value">от 70 000 ₽</div><div class="salary-label">Амурская область (начальный)</div></div>
                    <div class="salary-item"><div class="salary-value">120–180 тыс. ₽</div><div class="salary-label">Опытный специалист</div></div>
                    <div class="salary-item"><div class="salary-value">до 300 000 ₽</div><div class="salary-label">Старший инженер / DevOps</div></div>
                </div>
                <div class="info-text" style="margin-top: 12px; font-size:0.85rem;">*Данные hh.ru, trudvsem.ru, 2026</div>
            </div>

            <div class="category-btns">
                <button class="cat-btn" data-cat="school">🎓 Школьник</button>
                <button class="cat-btn" data-cat="parent">👪 Родитель</button>
                <button class="cat-btn" data-cat="job">💼 Ищу работу</button>
            </div>

            <div id="questionsArea"></div>
            <button id="nextToMapBtn" class="next-btn" style="display: none;">🚀 Узнать свой этап →</button>
        </div>
    </div>

    <!-- СТРАНИЦА 2: МАРШРУТНАЯ КАРТА -->
    <div id="pageMap" class="hidden">
        <div class="card">
            <button id="backToSurveyBtn" class="back-btn">← Пройти опрос заново</button>
            <h2>🗺️ Ваша карьерная карта <span class="badge" id="userRoleBadge"></span></h2>
            <div id="recommendBlock" class="recommend-block">
                <div class="recommend-label">🎯 Рекомендованный старт:</div>
                <div id="recommendStage" class="recommend-stage-name"></div>
                <div id="recommendText" class="recommend-text"></div>
            </div>
            <div id="fullMap" class="map-grid"></div>
            <div class="footer-note">🌐 При поддержке нацпроекта «Дети и молодёжь», «Профессионалитет», «Код будущего», «Работа в России»</div>
        </div>
    </div>
</div>

<script>
    const stages = [
        { id:1, title:"📚 Школьная база", desc:"Математика, информатика, английский. Участвуй в олимпиадах.", links:[
            { name:"Код будущего", url:"https://www.gosuslugi.ru/futurecode" },
            { name:"Stepik — бесплатные курсы", url:"https://stepik.org/catalog/search?free=true" },
            { name:"Учи.ру", url:"https://uchi.ru" }
        ]},
        { id:2, title:"🧪 IT-пробы и кружки", desc:"Кванториум, IT-куб, Билет в будущее. Пробуй себя в сетях.", links:[
            { name:"Навигатор допобразования", url:"https://dopportal.amurobl.ru/?municipality=1" },
            { name:"Кванториум-28", url:"https://kvantorium-28.ru/" },
            { name:"IT-куб", url:"https://it-cube28.ru/" },
            { name:"Билет в будущее", url:"https://bvbinfo.ru/" }
        ]},
        { id:3, title:"🏫 СПО / Профессионалитет", desc:"Специальность 09.02.06. Очное/заочное от 1 года 10 мес. Целевое обучение.", links:[
            { name:"Колледжи Профессионалитета", url:"https://япроф.рф/objects/?arrFilter_17_2944839123=Y&set_filter=Y" },
            { name:"Амурский колледж строительства и ЖКХ", url:"https://akszkh.ru/" },
            { name:"Благовещенский политехнический колледж", url:"https://polyt-amur.ru/" },
            { name:"Целевое обучение", url:"https://trudvsem.ru/target-education/search" }
        ]},
        { id:4, title:"🛠️ Практика на объектах", desc:"Стажировки на предприятиях Амурской области. Оплачивается!", links:[
            { name:"ЦОПП для студентов", url:"https://amurcopp.ru/бцк-для-студентов/" },
            { name:"Вакансии стажёров", url:"https://trudvsem.ru" }
        ]},
        { id:5, title:"📜 Курсы & сертификация (Отечественное ПО)", desc:"Бесплатные курсы Astra Linux, РЕД СОФТ, Kaspersky, Альт ОС, Postgres Pro.", links:[
            { name:"Astra Linux обучение", url:"https://astralinux.ru/training/" },
            { name:"РЕД СОФТ", url:"https://red-soft.ru/education" },
            { name:"Kaspersky Academy", url:"https://academy.kaspersky.ru/courses/" },
            { name:"Basalt SPO (Альт ОС)", url:"https://basealt.ru/education" },
            { name:"Postgres Pro", url:"https://postgrespro.ru/education" }
        ]},
        { id:6, title:"💼 Карьера на объектах региона", desc:"Трудоустройство: сетевой инженер, специалист по Astra Linux, DevOps. Зарплата от 80 000 ₽.", links:[
            { name:"Работа в России", url:"https://trudvsem.ru" },
            { name:"HeadHunter", url:"https://hh.ru" }
        ]}
    ];

    let currentCategory = "school";
    let answers = { school: null, parent: null, job: null };

    function determineStage(category, answerValue) {
        if (category === "school") return answerValue === "8-9" ? 1 : 2;
        if (category === "parent") {
            if (answerValue === "до 14") return 1;
            if (answerValue === "14-17") return 2;
            return 3;
        }
        if (category === "job") {
            if (answerValue === "нет опыта и знаний") return 3;
            if (answerValue === "базовый") return 4;
            return 6;
        }
        return 1;
    }

    function scrollToQuestionsAndHighlight() {
        const questionBlock = document.getElementById('activeQuestionBlock');
        if (questionBlock) {
            questionBlock.classList.add('question-highlight');
            setTimeout(() => questionBlock.classList.remove('question-highlight'), 800);
            questionBlock.scrollIntoView({ behavior: 'smooth', block: 'center' });
        }
    }

    function renderQuestionsAndScroll() {
        const container = document.getElementById("questionsArea");
        const nextBtn = document.getElementById("nextToMapBtn");
        if (!container) return;

        if (currentCategory === "school") {
            container.innerHTML = `<div class="question" id="activeQuestionBlock"><p>🎓 В каком ты классе?</p><div class="option-row"><div class="option-btn" data-val="8-9">8–9 класс</div><div class="option-btn" data-val="10-11">10–11 класс</div></div></div>`;
        } else if (currentCategory === "parent") {
            container.innerHTML = `<div class="question" id="activeQuestionBlock"><p>👪 Сколько лет вашему ребёнку?</p><div class="option-row"><div class="option-btn" data-val="до 14">До 14 лет</div><div class="option-btn" data-val="14-17">14–17 лет</div><div class="option-btn" data-val="18+">18+ (студент)</div></div></div>`;
        } else if (currentCategory === "job") {
            container.innerHTML = `<div class="question" id="activeQuestionBlock"><p>💼 Какой у вас опыт и знания в IT?</p><div class="option-row"><div class="option-btn" data-val="нет опыта и знаний">Нет опыта и знаний в IT</div><div class="option-btn" data-val="базовый">Базовые знания (ПК, интернет)</div><div class="option-btn" data-val="профильный">Профильный опыт (сети, администрирование)</div></div></div>`;
        }

        document.querySelectorAll('.option-btn').forEach(btn => {
            btn.addEventListener('click', () => {
                document.querySelectorAll('.option-btn').forEach(b => b.classList.remove('selected'));
                btn.classList.add('selected');
                answers[currentCategory] = btn.getAttribute('data-val');
                document.getElementById("nextToMapBtn").style.display = 'block';
            });
        });

        setTimeout(() => scrollToQuestionsAndHighlight(), 100);
    }

    function initCategoryButtons() {
        document.querySelectorAll('.cat-btn').forEach(btn => {
            btn.addEventListener('click', () => {
                document.querySelectorAll('.cat-btn').forEach(b => b.classList.remove('active'));
                btn.classList.add('active');
                currentCategory = btn.getAttribute('data-cat');
                answers[currentCategory] = null;
                renderQuestionsAndScroll();
                document.getElementById("nextToMapBtn").style.display = "none";
            });
        });
    }

    function goToMap() {
        const answer = answers[currentCategory];
        if (!answer) { alert("Пожалуйста, выберите вариант"); return; }
        const stageId = determineStage(currentCategory, answer);
        showMapPage(stageId, currentCategory, answer);
    }

    function showMapPage(recommendedStage, category, answerRaw) {
        document.getElementById("pageSurvey").classList.add("hidden");
        document.getElementById("pageMap").classList.remove("hidden");

        const roleMap = { school:"Школьник", parent:"Родитель", job:"Ищу работу" };
        document.getElementById("userRoleBadge").innerText = roleMap[category];
        const stageObj = stages.find(s => s.id === recommendedStage);
        document.getElementById("recommendStage").innerHTML = stageObj ? stageObj.title : "Этап 1";

        let recMsg = "";
        if (category === "school") recMsg = "Начните с изучения базовых IT-дисциплин и проекта «Код будущего».";
        else if (category === "parent") recMsg = "Помогите ребёнку записаться на бесплатные курсы и профпробы.";
        else if (category === "job") {
            if (answerRaw === "нет опыта и знаний") recMsg = "⭐ Рекомендуем начать с заочного обучения в СПО по специальности 09.02.06. Совмещайте работу и учёбу.";
            else if (answerRaw === "базовый") recMsg = "У вас есть база! Рекомендуем этап «Практика» — стажировки на предприятиях.";
            else recMsg = "С вашим опытом можно сразу переходить к этапу «Карьера». Изучайте вакансии.";
        }
        document.getElementById("recommendText").innerHTML = recMsg;

        const mapContainer = document.getElementById("fullMap");
        mapContainer.innerHTML = "";
        stages.forEach(stage => {
            const isRecommended = stage.id === recommendedStage;
            const div = document.createElement("div");
            div.className = "map-stage";
            if (isRecommended) div.style.borderLeftColor = "#f39c12";
            div.innerHTML = `
                <div class="stage-header"><span class="stage-number">${stage.id}</span><span class="stage-title">${stage.title}</span>${isRecommended ? '<span class="badge">⭐ Ваш этап</span>' : ''}</div>
                <div class="stage-desc">${stage.desc}</div>
                <div class="links">${stage.links.map(l => `<a href="${l.url}" target="_blank" class="link-btn">🔗 ${l.name}</a>`).join('')}</div>
            `;
            mapContainer.appendChild(div);
        });
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    function backToSurvey() {
        document.getElementById("pageMap").classList.add("hidden");
        document.getElementById("pageSurvey").classList.remove("hidden");
        answers[currentCategory] = null;
        renderQuestionsAndScroll();
        document.getElementById("nextToMapBtn").style.display = "none";
        window.scrollTo({ top: 0, behavior: 'smooth' });
    }

    function resetAndStart() {
        currentCategory = "school";
        answers = { school: null, parent: null, job: null };
        document.querySelectorAll('.cat-btn').forEach(btn => btn.classList.remove('active'));
        document.querySelector('.cat-btn[data-cat="school"]').classList.add('active');
        renderQuestionsAndScroll();
        document.getElementById("nextToMapBtn").style.display = "none";
        document.getElementById("pageMap").classList.add("hidden");
        document.getElementById("pageSurvey").classList.remove("hidden");
    }

    document.addEventListener("DOMContentLoaded", () => {
        initCategoryButtons();
        renderQuestionsAndScroll();
        document.getElementById("nextToMapBtn").addEventListener("click", goToMap);
        document.getElementById("backToSurveyBtn").addEventListener("click", backToSurvey);
        resetAndStart();
    });
</script>
</body>
</html>
