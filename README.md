
-Выполнен рефакторинг CSS-кода проекта используя препроцессор SASS.

-В корне проэкта созданна скрытая папка- .vscode в папке созданна еще одна папка- settings.json в которую загружаем настройки.

-Перед названии паршала ставим нижнее подчеркивание _  и ставим расширение scss.

-Все паршалы импортированны в main.scss  @import "./"; можно без нижнего подчеркивания и расширения.

-Соблюденна каскадность.

-Все паршалы лежат в отдельных папках:  

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



