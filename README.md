# 13.04-02
Пирамида тестирования

Занятие: Пирамида тестирования

	Содал репозиторий на GitHub, клонировал себе на ПК(в Git Bash Here):
git clone https://github.com/Al101010/13.04-02.git

	перешёл в него:
cd 13.04-02

	=> скопировал туда листинг занятия.
	=> в терминале Visual Studio Code сделал установку:
npm install
	появилась папка node_modules.

	=> поправил index.html:
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>13.04-02</title>
</head>

<body>
    <!-- TODO: comment after component added -->
    <form class="innogrn-form-widget">
        <div class="form-control">
            <label for="innorgn-input">Введите ИНН/ОГРН</label>
            <input id="innorgn-input" data-id="innorgn-input" type="text">
        </div>
        <button data-id="innorgn-input">Далее</button>
    </form>
    <div class="container"></div>
</body>

</html>

	=> запустил сборку проекта:
npm run build
	появилась папка dist.

	=> запустил live-server:
npm run show:dist

	=>   -= Появилось две формы на странице, index.html вернул старый. ИТОГ: форма одна. =- (удалил widget.test.js)
npm run test

	=> Покрытие провелил:
npm run coverage
