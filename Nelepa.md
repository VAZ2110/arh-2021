# Лабораторна робота №1
### Тема: Выбор команд RISC та CISC
### Мета: составить набранные командные RISC и CISC, заявить основную теоретическую информацию.
## Хід роботи
Діаграма порівняння RISC та CISK
| Основа для порівняння | RISC | CISK |
| -----------------|-----------| -----------|
| Наголос (основа на чому базується) | Програмне забезпечення | Устаткування |
| Розмір набору інструкцій | Малий | Великий |
| Включає |Один годинник | Багато годинник
| Формати інструкцій | Фіксований (32-бітний) формат | Різні формати (16-64 біт кожної інструкції). |
| Використовуються режими адресації | Обмежено до 3-5 |12-24 |
| Використовуються регістри загального призначення  | 32-192 | 8-24 |
| Висновки пам'яті | Зареєструйтеся для реєстрації | Пам'ять в пам'ять |
| Дизайн кешу | Розділити кеш даних і кеш інструкцій. | Єдиний кеш для інструкцій і даних |
| Тактова частота (типові)| 50-150 МГц | 33-50 МГц |
| Цикли на інструкцію | Єдиний цикл для всіх інструкцій і середній ІСЦ <1.5. |ІСЦ між 2 і 15. |
| Керування процесором | Обмотка без пам'яті управління | Мікрокодування с использованием керуючої пам'яті (ПЗУ) |

### Висновок
Інструкції CISC є складними і мають тенденцію до уповільнення, ніж RISC, але використовують менше циклів з меншою кількістю інструкцій.

### Контрольні питання
##### 1. Коротко охарактеризуйте набір команд RISC?
Набори команд зі зменшеними наборами команд (RISC), як правило, містять менше 100 інструкцій і використовують фіксований формат інструкцій (32 біта). Він використовує кілька простих режимів адресації. Використовуються інструкції на основі реєстру, що означає, що використовується механізм реєстрації для реєстрації. LOAD / STORE - єдині незалежні інструкції для доступу до пам'яті.
Для підвищення швидкості перемикання контекстів використовується великий файл реєстру. Простота наборів команд призвела до реалізації цілих процесорів на одному чіпі VLSI. Додатковими перевагами є більш висока тактова частота, нижчий ІСЦ, що регулюють високі рейтинги MIPS на наявних RISC / суперскалярних процесорах.

##### 2. Коротко охарактеризуйте набір команд CISC?
Комплекс команд набору команд (CISC) набір інструкцій містить близько 120 до 350 інструкцій. Він використовує змінні формати інструкцій / даних, але невеликий набір регістрів загального призначення, тобто 8-24. Причиною великих наборів команд є використання інструкцій змінного формату. Велика кількість еталонних операцій пам'яті виконується за допомогою величезної кількості режимів адресації.
Архітектура CISC безпосередньо використовує оператори HLL в апаратних / прошивках. Єдиний кеш використовується в традиційній архітектурі CISC, яка містить як дані, так і інструкції, і використовує загальний шлях.

##### 3. Дайте портирование набора команд.

* У RISC розмір набору команд невеликий, а в CISC величина набору команд велика.
* RISC определяет форматы форматов (32 бита) и в основном региональные структуры, этот вариант CISC предлагает варианты форматов от 16 до 64 байт на структуре.
* RISC-використов один годинник и обмежений режим адресов (тобто 3-5). С иностранного адреса, CISC использует дату от 24 до 24 режимов адреса.
* Качество регенерации загального значения, распознавания RISC, действует от 32-192. Навпаки, архітектура CISC використовує 8-24 GPR.
* Механізм реєстрації в регістр використовться в RISC з незалежными структурами LOAD і STORE. На відміну від цього, CISC використову механізм пам'яті до пам'яті для виконання
операцій, крім того, включені структуры ЗАГРУЗИТЬ і МАГАЗИН.
* RISC предоставляет данные и инструкции по обучению. На відміну від цього, CISC використовую уніфікований кеш для даних и конструкцій, хочется останні конструкції такожаж використовують розділені кеші.
* Більшість элементов керування процесором в RISC є провідними без наявності пам'яті керування. І навпаки, CISC мікрокодується и використовує керуючу пам'ять (ROM), але сучасний CISC також використовує жорстке керування.
