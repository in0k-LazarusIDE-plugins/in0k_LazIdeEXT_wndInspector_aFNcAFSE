# wndInspector_FF8S

[Эксперт][D1] для среды разработки [Lazarus IDE][D2].

## Добавляемые функции IDE
  Поиск файла из "[Редактора Исходного Кода][l0]", в открытых окнах "Инспекторах"
  ("[Инспектор Проекта][l1]", "[Редактор Пакета][l2]").

### Проявление
  Установка фокуса на узел "Дерева Зависимостей" окна "Инспектора", в 
  соответствии с текущим [активным][l3] файлом в окне "Редактора Исходного Кода".
  
  Визуальную демонстрацию работы компонента вы можете увидеть в анимации
  [Команда IDE](https://github.com/in0k-LazarusIDE-plugins/in0k_LazIdeEXT_wndInspector_FF8S/wiki/Animation-'IDE-command')
  и
  [Автоматический режим](https://github.com/in0k-LazarusIDE-plugins/in0k_LazIdeEXT_wndInspector_FF8S/wiki/Animation-'Auto-MODE').



### Возможности

* Команда IDE
  - горячая клавиша: `Ctrl`+`Shift`+`Alt`+`F` (для изменения см. [Shortcuts][l4])
  - пункт меню: `IDE menu`->`Search`->`Find File in "Inspector"`
  - пункт меню: `Source editor`->`Рopup menu`->`Find File in "Inspector"`
  - дополнительно:
    + перемещение окна "Инспектора", в котором найден файл, на "Передний План"
    + сообщение, если файл не найден ни в одном из открытых окон "Инспекторов"
* Автоматический режим
   - поиск запускается при изменении "[Активного Редактора Исходных Кодов][l3]"
   - дополнительно:
     + перемещение окна "Инспектора", в котором найден файл, на 
       "[Второй План](https://github.com/in0k-src/in0k-bringToSecondPlane)"
       (это хорошо работает в системах Windows. Для других систем эта опция по умолчанию НЕ включенна, так как приводит к "морганию" интерфейса)
     + сохранение состояния свернутых узлов в "Дереве Зависимостей"
     + визуальное выделение активного узла в "Дереве Зависимостей"
     + "миниКарта" для Выделенного и Активного узла в "Дереве Зависимостей"
* "Дерево Зависимостей" окна "Инспектора"
  + дополнительные пункты контекстного меню из серии "Свернуть ВСЕ"


## Установка и Настройка
* **Получение исходников**: "клонируйте" репозиторий со ВСЕМИ под проектами или
  скачайте ПОЛНЫЙ архив пакета (`.._fullSRC.zip`) из последнего 
  [релиза](https://github.com/in0k-LazarusIDE-plugins/in0k_LazIdeEXT_wndInspector_FF8S/releases). 
* **Установка**: используется [стандартная схема][I0] установки пакетов.
* **Настройка**: перед "сборкой" пакета отредактируйте файл `in0k_lazExt_SETTINGs.inc`.

[D1]: http://wiki.lazarus.freepascal.org/Extending_the_IDE#Overview
[D2]: http://www.lazarus-ide.org/ 
[I0]: http://wiki.freepascal.org/Install_Packages#Adding_known_packages
[l0]: http://wiki.freepascal.org/IDE_Window:_Source_Editor
[l1]: http://wiki.freepascal.org/IDE_Window:_Project_Inspector
[l2]: http://wiki.freepascal.org/IDE_Window:_Package_Editor
[l3]: http://wiki.freepascal.org/Extending_the_IDE#Active_source_editor
[l4]: http://wiki.freepascal.org/Lazarus_IDE_Shortcuts
