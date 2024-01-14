# Проект PyGame: Wild West



### Выполнили: Соколенко Дарья и Краснопольская Полина

---

Wild West - это игра файтинг в стиле дикого запада, в которой происходит бой между двумя персонажами. На одной стороне стоит первый герой, 
а на другой — второй. Цель каждого игрока - убить противника с минимальными потерями здоровья для себя. 
Игра предполагает участие двух человек.

---

## Правила:
При запуске приложения игрок попадает в главное меню. Чтобы начать играть, человеку нужно авторизоваться, нажав для этого соответсвующую кнопку.
После авторизации выбрать уровень. На каждом уровне битва состоит из трех раундов. Побеждает тот, кто одержал победу в наибольшом количестве раундов.
После окончания игры можно начать заново, выбрав любой уровень.

* **Доступные уровни**:

  - Легкий

  - Средний

  - Сложный

На каждом уровне свой фон и звук игры. С увеличением сложности уровня уменьшается урон, наносимый при ударе противнику.
Становится сложнее убить, длительность раунда увеличивается.
* **Управление**:


|              | Игрок слева | Игрок справа  |
|:-------------|:-----------:|:-------------:|
| **Движение** |    A W D    |     < ^ >     |
| **Удар**     |   R или T   |    O или P    |
           

--- 

## Структура

> папка `assets` - данные, необходимые для работы программы
>> база данных `login.db` - хранение информации об авторизации пользователей (находится в папке `assets`)
>
> папка `classes` - файлы Python, в которых хранятся классы, необходимые для работы программы
> 
> папка `ui` - папка, в которой хранятся ui - файлы, отвечающие за интерфейс окон PyQt ('WildWest' (начальное окно), 'SIGNUP' (окно регистрации), 'pravila' (окно с правилами игры), 'YROVEN' (окно выбора уровня))

| Название класса |                                            Содержание                                             |
|:----------------|:-------------------------------------------------------------------------------------------------:|
| Login_db        |                     создание и управление базой данных авторизации 'login.db'                     |
| Home            |            управление входом в игру и кнопками на начальном окне программы 'WildWest'             |
| Player          | движение и управление героем в игре, различные команды, относящиеся к нему (атаки, смерть и т.д.) |
| Signup          |              управление регистрацией (занесение нового пользователя в бд 'login.db')              |
| Yrovni          |                                 выбор уровня и вход в игру Pygame                                 |


___
<h3>Структура папки assets:</h3>
___

| Название папки | Содержание                                                  |
|:--------------:|-------------------------------------------------------------|
|     fonts      | В директории хранится шрифт, используемый в игре            |
|     images     | В директории хранятся изображения, используемые в программе |
|     audio      | В директории хранятся звуки и музыка, используемые в игре   |

---

#### Все окна, кроме игровых, написаны с использованием библиотеки PyQt5, игровые - PyGame.

---

## Запуск

- основной исполняемый файл программы `main.py`
- необходимые зависимости созданы в файле `requirements.txt`, команда для установки зависимостей - `pip install -r requirements.txt`


## Перспективы развития

- выбор персонажа, за которого будешь играть
- выбор оружия, которым будешь играть
- таблица лидеров по количеству побед
- таймер на раунд, если раунд не закончился, побеждает тот, у кого больше здоровья
- выбор режима игры: один или двое, если один, то за противника играет компьютер

### Программные окна

- *Главное окно*
![img.png](assets/images/readme/img.png)

- *Окно авторизации*
![img_1.png](assets/images/readme/img_1.png)

- *Окно с правилами игры*
![img_6.png](assets/images/readme/img_6.png)

- *Окно выбора уровня*
![img_2.png](assets/images/readme/img_2.png)

- *Окно легкого уровня*
![img_4.png](assets/images/readme/img_4.png)

- *Окно среднего уровня*
![img_3.png](assets/images/readme/img_3.png)

- *Окно сложного уровня*
![img_5.png](assets/images/readme/img_5.png)
