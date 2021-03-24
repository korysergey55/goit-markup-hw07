
1.Выполнен рефакторинг CSS-кода проекта используя препроцессор SASS.

2.В корне проэкта созданна скрытая папка- .vscode в папке созданна еще одна папка- settings.json в которую загружаем настройки:
{
    "liveSassCompile.settings.formats": [
        {
            "format": "expanded",
            "extensionName": ".css",
            "savePath": "/css"
        },
        {
            "format": "compressed",
            "extensionName": ".min.css",
            "savePath": "/css"
        }
    ],
    "liveSassCompile.settings.excludeList": [
        "**/node_modules/**",
        ".vscode/**"
    ],
    "liveSassCompile.settings.generateMap": true,
    "liveServer.settings.port": 1235,
    "liveSassCompile.settings.autoprefix": null
}

3.Перед названии паршала ставим нижнее подчеркивание _  и ставим расширение scss.

4.Все паршалы импортированны в main.scss через @import "./"; 

@import "./utils/variables";
@import "./utils/visually-hidden";
/* ===========BASE===========*/
@import "./base/common";
@import "./base/container";
/* =========== COMPONENTNS ===========*/
@import "./components/section";
@import "./components/title";
@import "./components/logo";
@import "./components/backdrop";
@import "./components/modal-form";
/* ===========LAYOUT===========*/
@import "./layout/header";
@import "./layout/hero";
@import "./layout/features";
@import "./layout/specialization";
@import "./layout/team";
@import "./layout/clients";
@import "./layout/footer";
@import "./layout/partfolio";



