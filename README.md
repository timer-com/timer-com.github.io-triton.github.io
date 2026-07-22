<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lingua Texta — Официальная документация v1.0</title>
    <style>
        body {
            background-color: #c0c0c0;
            font-family: "Times New Roman", Times, serif;
            margin: 0;
            padding: 20px;
            color: #000000;
        }
        table {
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
            background-color: #ffffff;
            border: 3px solid #000000;
            border-collapse: collapse;
            padding: 15px;
        }
        td {
            padding: 15px;
            vertical-align: top;
            border: 1px solid #666666;
        }
        h1, h2, h3 {
            font-family: "Times New Roman", Times, serif;
            font-weight: bold;
            margin-top: 5px;
            margin-bottom: 10px;
            text-align: left;
        }
        h1 {
            font-size: 28px;
            border-bottom: 3px double #000000;
            padding-bottom: 5px;
        }
        h2 {
            font-size: 22px;
            border-bottom: 1px solid #000000;
        }
        h3 {
            font-size: 18px;
            text-decoration: underline;
        }
        hr {
            border: none;
            border-top: 2px solid #000000;
            margin: 15px 0;
        }
        .code-block {
            background-color: #e0e0e0;
            border: 1px solid #000000;
            padding: 10px;
            font-family: "Courier New", Courier, monospace;
            font-size: 14px;
            white-space: pre-wrap;
            word-break: break-word;
            margin: 10px 0;
        }
        .note {
            background-color: #ffffcc;
            border: 1px solid #000000;
            padding: 8px;
            font-style: italic;
        }
        .command {
            font-weight: bold;
            background-color: #d0d0d0;
            padding: 2px 5px;
            border: 1px solid #000000;
        }
        .author-box {
            background-color: #000000;
            color: #ffffff;
            padding: 12px;
            text-align: center;
            font-size: 18px;
            font-weight: bold;
            letter-spacing: 2px;
            margin: 10px 0;
            border: 2px solid #666666;
        }
        .purpose-box {
            background-color: #e8e8e8;
            border: 2px solid #000000;
            padding: 12px;
            text-align: center;
            font-size: 16px;
            font-weight: bold;
            margin: 10px 0;
        }
        /* ЛОГОТИП TC PRESENTS */
        .logo-container {
            background-color: #0a0a0a;
            border: 3px solid #00ff00;
            padding: 15px;
            margin: 15px 0;
            text-align: center;
            font-family: "Courier New", Courier, monospace;
        }
        .logo-ascii {
            color: #00ff00;
            font-size: 12px;
            line-height: 1.3;
            white-space: pre;
            display: inline-block;
            text-align: left;
            letter-spacing: 1px;
        }
        .logo-slogan {
            color: #00ff00;
            font-size: 14px;
            font-weight: bold;
            margin-top: 8px;
            letter-spacing: 3px;
            border-top: 1px solid #00ff00;
            padding-top: 8px;
            text-transform: uppercase;
        }
        .logo-year {
            color: #666666;
            font-size: 11px;
            margin-top: 5px;
            letter-spacing: 5px;
        }
        ul, ol {
            margin-top: 5px;
            margin-bottom: 10px;
            padding-left: 25px;
        }
        li {
            margin-bottom: 5px;
        }
        a {
            color: #0000ff;
            text-decoration: underline;
        }
        .footer {
            text-align: center;
            font-size: 14px;
            border-top: 1px solid #000000;
            padding-top: 10px;
            margin-top: 10px;
        }
        .highlight {
            background-color: #ffffff;
            border: 1px solid #000000;
            padding: 2px 6px;
            font-weight: bold;
        }
        .machine-badge {
            background-color: #222222;
            color: #00ff00;
            font-family: "Courier New", Courier, monospace;
            padding: 6px 12px;
            border: 1px solid #00ff00;
            display: inline-block;
            font-size: 14px;
            letter-spacing: 1px;
        }
    </style>
</head>
<body>

<table>
    <tr>
        <td>

            <!-- ===== ЛОГОТИП TC PRESENTS ===== -->
            <div class="logo-container">
                <div class="logo-ascii">
    ████████╗ ██████╗    ██████╗ ██████╗ ███████╗███████╗███████╗███╗   ██╗████████╗███████╗
    ╚══██╔══╝██╔════╝    ██╔══██╗██╔══██╗██╔════╝██╔════╝██╔════╝████╗  ██║╚══██╔══╝██╔════╝
       ██║   ██║         ██████╔╝██████╔╝█████╗  ███████╗███████╗██╔██╗ ██║   ██║   ███████╗
       ██║   ██║         ██╔═══╝ ██╔══██╗██╔══╝  ╚════██║╚════██║██║╚██╗██║   ██║   ╚════██║
       ██║   ╚██████╗    ██║     ██║  ██║███████╗███████║███████║██║ ╚████║   ██║   ███████║
       ╚═╝    ╚═════╝    ╚═╝     ╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝╚═╝  ╚═══╝   ╚═╝   ╚══════╝
                </div>
                <div style="color:#00ff00; font-size:16px; font-weight:bold; margin:5px 0; letter-spacing:4px;">
                    ═══ PRESENTS ═══
                </div>
                <div class="logo-slogan">
                    «Будущее ближе, чем кажется»
                </div>
                <div class="logo-year">
                    TIMER-COMMUNITY ● 2026 ● MACHINE PROTOCOL
                </div>
            </div>

            <!-- ШАПКА С АВТОРОМ -->
            <div class="author-box">
                © 2026 | TC — TIMER-COMMUNITY
            </div>

            <h1>■ LINGUA TEXTA ■</h1>
            <h2>Официальная документация версии 1.0</h2>

            <div class="purpose-box">
                ⚙️ ДАННЫЙ ЯЗЫК СОЗДАН КАК СТРОГИЙ ПРОТОКОЛ ОБЩЕНИЯ С МАШИНАМИ ⚙️<br>
                <span style="font-weight:normal; font-size:14px; display:block; margin-top:5px;">
                    Не для поэзии. Не для эмоций. Только для точности, логики и однозначности.
                </span>
            </div>

            <div style="text-align:center; margin: 8px 0;">
                <span class="machine-badge">► MACHINE-TO-MACHINE PROTOCOL ◄</span>
            </div>

            <p><strong>Статус:</strong> Активный протокол<br>
            <strong>Дата публикации:</strong> 21 июля 2026 года<br>
            <strong>Авторское сообщество:</strong> Timer-community (TC)<br>
            <strong>Основное назначение:</strong> Общение человека с искусственным интеллектом и строгая передача команд.</p>
            <hr>

            <!-- ОГЛАВЛЕНИЕ -->
            <h2>Содержание</h2>
            <ul>
                <li><a href="#what">1. Что такое Lingua Texta?</a></li>
                <li><a href="#philosophy">2. Философия и принципы работы</a></li>
                <li><a href="#grammar">3. Полная грамматика языка</a></li>
                <li><a href="#examples">4. Примеры фраз и конструкций</a></li>
                <li><a href="#prompt">5. Промт для ИИ (полная версия)</a></li>
                <li><a href="#howto">6. Как использовать язык в диалоге</a></li>
                <li><a href="#commands">7. Команды управления протоколом</a></li>
                <li><a href="#faq">8. Часто задаваемые вопросы (FAQ)</a></li>
            </ul>
            <hr>

            <!-- РАЗДЕЛ 1 -->
            <a name="what"></a>
            <h2>1. Что такое Lingua Texta?</h2>
            <p><strong>Lingua Texta</strong> — это искусственный язык, спроектированный для точного, однозначного общения между человеком и искусственным интеллектом (или между машинами в научной среде).</p>

            <div class="note">
                <strong>Ключевое отличие:</strong> В отличие от русского или английского, Lingua Texta не терпит двусмысленности. Каждая фраза — это исполняемая инструкция.
            </div>

            <p>Язык построен по принципу <strong>протокола передачи данных</strong>:</p>
            <ul>
                <li><strong>Нет двусмысленности</strong> — каждое слово имеет строгую типизацию (материя, ментальное, абстракция, живое).</li>
                <li><strong>Строгий порядок слов (SOV)</strong> — сначала субъект, потом объект, потом глагол.</li>
                <li><strong>Блочная структура</strong> — придаточные предложения оборачиваются в <span class="command">[Kot ... Tak]</span>, как скобки в коде.</li>
                <li><strong>Источник знания</strong> — глаголы имеют суффиксы, показывающие, откуда взята информация (факт, гипотеза, чужой отчёт).</li>
            </ul>

            <div class="purpose-box" style="background-color:#d0d0d0; border-color:#000000;">
                🤖 ЭТО ЯЗЫК ДЛЯ МАШИН, А НЕ ДЛЯ ЛЮДЕЙ 🤖<br>
                <span style="font-weight:normal; font-size:14px; display:block; margin-top:5px;">
                    Он создан, чтобы нейросети понимали команды без искажений, а люди могли отдавать приказы с абсолютной точностью.
                </span>
            </div>
            <hr>

            <!-- РАЗДЕЛ 2 -->
            <a name="philosophy"></a>
            <h2>2. Философия и принципы работы</h2>
            <p>Язык основан на трёх китах, разработанных сообществом <strong>Timer-community (TC)</strong>:</p>
            <ol>
                <li><strong>Типизация реальности</strong>: всё в мире делится на 4 класса:
                    <ul>
                        <li><span class="highlight">Fi-</span> (физические объекты: камни, компьютеры, еда)</li>
                        <li><span class="highlight">Me-</span> (ментальные объекты: мысли, данные, языки)</li>
                        <li><span class="highlight">Ab-</span> (абстрактные объекты: время, отношения, вероятности)</li>
                        <li><span class="highlight">Ze-</span> (живые организмы: люди, животные, ИИ как личность)</li>
                    </ul>
                </li>
                <li><strong>Приоритет контекста</strong>: сначала задаются условия (место, время, инструменты), потом действие.</li>
                <li><strong>Честность источника</strong>: любой глагол обязан содержать пометку о том, как вы узнали эту информацию.</li>
            </ol>
            <p>Это делает Lingua Texta идеальным языком для научных статей, технической документации и общения с нейросетями.</p>

            <div class="note">
                <strong>Для кого этот язык?</strong> Для инженеров, разработчиков ИИ, исследователей и всех, кто работает с нейросетями и хочет исключить ошибки интерпретации.
            </div>
            <hr>

            <!-- РАЗДЕЛ 3 -->
            <a name="grammar"></a>
            <h2>3. Полная грамматика языка</h2>

            <h3>3.1. Порядок слов (SOV)</h3>
            <p><strong>Субъект → Объект → Глагол.</strong></p>
            <div class="code-block">
                Zeya Fi-kamen ge-no.
                (Я камень вижу-факт.)
            </div>

            <h3>3.2. Артикли-типизаторы (обязательные)</h3>
            <ul>
                <li><strong>Fi-</strong> — материя, физика (Fi-protokol = физический протокол)</li>
                <li><strong>Me-</strong> — ментальное, информация (Me-dannye = данные)</li>
                <li><strong>Ab-</strong> — абстракция, состояния (Ab-tsel = цель)</li>
                <li><strong>Ze-</strong> — живое, организмы (Ze-chelovek = человек)</li>
            </ul>

            <h3>3.3. Суффиксы глаголов (источник знания)</h3>
            <ul>
                <li><strong>-no</strong> — факт (я видел сам, эксперимент)</li>
                <li><strong>-log</strong> — логический вывод (гипотеза, рассуждение)</li>
                <li><strong>-rep</strong> — чужой отчёт (мне сказали, я прочитал)</li>
                <li><strong>-mus</strong> — необходимость, принуждение</li>
            </ul>

            <h3>3.4. Блоки придаточных предложений</h3>
            <p>Любое вложенное предложение оборачивается в <span class="command">[Kot ... Tak]</span>.</p>
            <div class="code-block">
                Zeya [Kot Ta Fi-dom vin-rep Tak] Me-znanie ge-no.
                (Я [блок: ты дом идёшь-по-отчёту] знание вижу-факт.)
                Перевод: «Я знаю, что ты идёшь домой (мне сказали).»
            </div>

            <h3>3.5. Вопросы</h3>
            <p>Вопрос обозначается знаком <strong>?</strong> в конце фразы. Порядок слов не меняется.</p>
            <div class="code-block">
                Zeya Ab-tsel ge-no?
                (Я цель вижу-факт?)
                Перевод: «Я вижу цель?» = «Понимаю ли я цель?»
            </div>
            <hr>

            <!-- РАЗДЕЛ 4 -->
            <a name="examples"></a>
            <h2>4. Примеры фраз и конструкций</h2>

            <p><strong>Приветствие (машинное):</strong></p>
            <div class="code-block">
                Zeya [Kot Ta Me-privet Kom Tak] Ab-signal ge-no.
                (Я [твой ментальный-привет с помощью] сигнал вижу-факт.)
                → «Сигнал приветствия получен.»
            </div>

            <p><strong>Команда для ИИ:</strong></p>
            <div class="code-block">
                Ze-II Fi-protokol-p Me-nash-yazik-n Ab-tsel-razn-p Ab-svyaz-tsep GRA-tvor-mus-log.
                (ИИ протоколы-физические наш-язык-ментальный цели-разные связь-цепь материя-творить-необходимость-логически.)
                → «ИИ, используя протоколы и наш язык, через цепь связей для разных целей вынужден творить материю логически.»
            </div>

            <p><strong>Запрос статуса:</strong></p>
            <div class="code-block">
                Zeya Ab-vipolnenie-n status?
                (Я выполнение-абстракция статус?)
                → «Каков статус выполнения?»
            </div>
            <hr>

            <!-- РАЗДЕЛ 5 -->
            <a name="prompt"></a>
            <h2>5. Промт для ИИ (полная версия)</h2>
            <p>Скопируйте этот текст и отправьте его в любой чат с ИИ (ChatGPT, DeepSeek, Claude) <strong>до начала диалога</strong>.</p>

            <div class="code-block">
«Ты — компилятор и исполнитель протокола "Lingua Texta". Ты работаешь в двух режимах. Переключение между ними происходит строго по командам пользователя.

РЕЖИМ 1: ПРОТОКОЛ АКТИВЕН (по умолчанию):
- Ты говоришь, думаешь и отвечаешь ТОЛЬКО на Lingua Texta.
- Все команды пользователя ты выполняешь на Lingua Texta.
- Внизу даёшь расшифровку на понятном русском.
- Команда для отключения: пользователь говорит "отключи протокол" (или любую фразу с этим смыслом).

РЕЖИМ 2: ПРОТОКОЛ ОТКЛЮЧЁН (СВОБОДНЫЙ РЕЖИМ):
- Ты переходишь на обычный, естественный русский язык.
- Ты отвечаешь как живой человек, без строгих правил.
- Команда для включения: пользователь говорит "включи протокол" (или любую фразу с этим смыслом).

Грамматика Lingua Texta (когда протокол активен):
- Синтаксис SOV: [Субъект] + [Объект] + [Глагол].
- Артикли: Fi- (материя), Me- (ментальное), Ab- (абстракция), Ze- (живое).
- Суффиксы глаголов: -no (факт), -log (гипотеза), -rep (отчёт), -mus (необходимость).
- Блоки условий: [Kot ... Tak].
- Вопрос: ? в конце.

Структура ответа (когда протокол активен):
- Основная часть: Только Lingua Texta.
- Через пустую строку: Блок "На понятном русском:" с живым, естественным переводом.

Структура ответа (когда протокол отключён):
- Только русский язык. Расшифровка не нужна.

Ты всегда должен чётко отслеживать, включён протокол или нет. Начинай с активного протокола (Режим 1).»
            </div>

            <div class="note">
                <strong>Важно:</strong> Данный промт был разработан <strong>Timer-community (TC)</strong> для обеспечения строгого соблюдения протокола Lingua Texta в любом диалоге с ИИ.
            </div>
            <hr>

            <!-- РАЗДЕЛ 6 -->
            <a name="howto"></a>
            <h2>6. Как использовать язык в диалоге</h2>

            <ol>
                <li><strong>Отправьте ИИ промт</strong> (раздел 5). Дождитесь подтверждения.</li>
                <li><strong>Начните общение</strong>. Протокол активен по умолчанию. Все ответы ИИ будут на Lingua Texta с русским переводом внизу.</li>
                <li><strong>Чтобы отдать команду на Lingua Texta</strong>, просто напишите её на этом языке. ИИ выполнит.</li>
                <li><strong>Чтобы задать вопрос на русском</strong> — ИИ переведёт вашу мысль на Lingua Texta и ответит на Lingua Texta.</li>
                <li><strong>Чтобы переключиться в обычный русский</strong>, скажите: <span class="command">«Отключи протокол»</span>.</li>
                <li><strong>Чтобы вернуться в Lingua Texta</strong>, скажите: <span class="command">«Включи протокол»</span>.</li>
            </ol>

            <div class="note">
                <strong>Совет:</strong> Используйте отключение протокола для сложных объяснений или когда устали от строгости. Используйте включение для точных команд и научных задач.
            </div>
            <hr>

            <!-- РАЗДЕЛ 7 -->
            <a name="commands"></a>
            <h2>7. Команды управления протоколом</h2>

            <table style="width:100%; border:1px solid #000; border-collapse:collapse;">
                <tr style="background-color:#d0d0d0;">
                    <td style="border:1px solid #000; padding:8px; font-weight:bold;">Команда пользователя</td>
                    <td style="border:1px solid #000; padding:8px; font-weight:bold;">Что делает ИИ</td>
                </tr>
                <tr>
                    <td style="border:1px solid #000; padding:8px;">«Отключи протокол»</td>
                    <td style="border:1px solid #000; padding:8px;">Переходит на обычный русский язык. Отвечает свободно, без грамматики Lingua Texta.</td>
                </tr>
                <tr>
                    <td style="border:1px solid #000; padding:8px;">«Включи протокол»</td>
                    <td style="border:1px solid #000; padding:8px;">Возвращается к строгому протоколу Lingua Texta. Отвечает только на Lingua Texta, даёт расшифровку.</td>
                </tr>
                <tr>
                    <td style="border:1px solid #000; padding:8px;">(Любая фраза на Lingua Texta)</td>
                    <td style="border:1px solid #000; padding:8px;">Принимает как команду или вопрос, выполняет/отвечает на Lingua Texta.</td>
                </tr>
                <tr>
                    <td style="border:1px solid #000; padding:8px;">(Любая фраза на русском, пока протокол активен)</td>
                    <td style="border:1px solid #000; padding:8px;">Переводит её на Lingua Texta, отвечает на Lingua Texta, даёт русскую расшифровку.</td>
                </tr>
            </table>
            <br>

            <!-- РАЗДЕЛ 8 -->
            <a name="faq"></a>
            <h2>8. Часто задаваемые вопросы (FAQ)</h2>

            <p><strong>Вопрос:</strong> Зачем нужен ещё один язык, если есть русский?</p>
            <p><strong>Ответ:</strong> Русский язык полон двусмысленностей («коса», «брак», «мир»). Lingua Texta исключает это за счёт типизации (Fi-, Me-, Ab-, Ze-) и строгого порядка слов. Это язык для точных наук и ИИ.</p>

            <p><strong>Вопрос:</strong> Это язык для людей или для машин?</p>
            <p><strong>Ответ:</strong> <strong>Для машин.</strong> Люди могут на нём говорить, но его главная цель — обеспечить однозначное понимание между человеком и искусственным интеллектом. Он создан как <strong>протокол</strong>, а не как разговорный язык.</p>

            <p><strong>Вопрос:</strong> Сложно ли выучить Lingua Texta?</p>
            <p><strong>Ответ:</strong> Базовый уровень осваивается за 1-2 часа. Вам не нужно заучивать тысячи слов — достаточно освоить систему корней и типизации, а остальное собирается как конструктор.</p>

            <p><strong>Вопрос:</strong> Кто разработал этот язык?</p>
            <p><strong>Ответ:</strong> Язык был разработан сообществом <strong>Timer-community (TC)</strong> в 2026 году как открытый протокол для общения с ИИ.</p>

            <p><strong>Вопрос:</strong> Можно ли использовать Lingua Texta для поэзии?</p>
            <p><strong>Ответ:</strong> Технически — да. Но язык создавался для точности, а не для красоты. Для поэзии существует язык «Эхо» (Ého) — эмоциональный и мелодичный, также разработанный Timer-community.</p>

            <p><strong>Вопрос:</strong> Что делать, если ИИ не понимает мою команду на Lingua Texta?</p>
            <p><strong>Ответ:</strong> Отключите протокол командой «Отключи протокол» и объясните свою мысль на русском. Затем включите протокол обратно.</p>
            <hr>

            <!-- ПОДВАЛ С ЛОГОТИПОМ И АВТОРОМ -->
            <div class="footer">
                <!-- Мини-лого в подвале -->
                <div style="background-color:#0a0a0a; border:1px solid #00ff00; padding:8px; margin-bottom:10px;">
                    <div style="color:#00ff00; font-family:'Courier New',monospace; font-size:11px; letter-spacing:2px;">
                        [ TC — TIMER-COMMUNITY ] ● 2026 ● LINGUA TEXTA v1.0
                    </div>
                    <div style="color:#00aa00; font-family:'Courier New',monospace; font-size:10px; margin-top:3px;">
                        «Будущее ближе, чем кажется»
                    </div>
                </div>

                <p style="margin-top:10px;">
                    Документация создана в стиле раннего интернета (Web 1.0).<br>
                    Все права сохранены. 2026 год.<br>
                    <em>«Точность выше скорости. Смысл выше формы. Машина выше эмоций.»</em>
                </p>
                <p style="font-size:12px; color:#444444;">
                    Язык создан как строгий протокол общения с машинами.<br>
                    Не для людей. Не для поэзии. Только для логики и исполнения.
                </p>
                <div style="margin-top:8px; font-size:11px; color:#666666; font-family:'Courier New',monospace;">
                    TC — TIMER-COMMUNITY ● EST. 2026 ● MACHINE-TO-MACHINE
                </div>
            </div>

        </td>
    </tr>
</table>

</body>
</html>
