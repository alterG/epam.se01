## **Homework for EPAM java course**  
Решения находятся в папке `src/`, задачи сопровождены readme с условиями.  
Для [задачи №6](https://github.com/alterG/javase01/tree/master/src/t06) добавлена видео-демонстрация, документацию можно [посмотреть онлайн](http://rubickcube.ru/epam/t06).    
- [X] Module #1
- [X] Module #2  
- [X] Module #3
- [X] Module #4 
- [ ] Module #5 

**Quizful.com**  
- [X] Main method, primitive types
- [X] Operators
- [X] If, else, switch and loops
- [X] Arrays
- [X] Keywords, OOP
- [ ] Input, Output, Collections, JVM  

**Codility.com**    
Решения находятся в папке `codility/lesson`, задачи сопровождены readme с условиями.  
- [X] BinaryGap
- [X] Arrays (2/2)
- [X] Time Complexity (3/3)
- [X] Counting Elements (4/4)
- [X] Prefix Sums (4/4)
- [X] Sorting (4/4)
- [X] Stacks and Queues (4/4)
- [X] Leader (2/2)
- [X] Maximum slice problem (3/3)
- [ ] Prime and composite numbers (3/4)

**Книги**
- [ ] Брюс Эккель - Философия Java `(162/1170)`  

**Доклады**  
* Вячеслав Круглов — Как начинающему Java-разработчику подружиться со своей базой данных? [ссылка](https://www.youtube.com/watch?v=dFASbaIG-UU) **(4/10)**
```
Оптимистичные, пессимистичные (read/write) блокировки, ORM, JPA, её реализации/провайдеры (Hibernate).  
```
* Владимир Иванов — G1 Garbage Collector. [ссылка](https://www.youtube.com/watch?v=iGRfyhE02lA) **(8/10)**
```
Слабая теория о поколениях, GC roots, STW-pause, object graph, Eden, FormSpace, ToSpace, Old Generation, Throughput-Latency-Footprint, STW-сборка против Инкрементальной, SerialGC, ParralelGC, CMS, G1б, -XX:+UseG1GC, -XX:MaxGCPauseMillis, -XX:GCPauseIntervalMillis.
```
* Егор Бугаенко — Объектно-ориентированное вранье. [ссылка](https://www.youtube.com/watch?v=lfdAwl3-X_c&t=3s) **(2/10)**
```
Getters, setters, static methods нарушают парадигму ООП, объект представляет самостоятельную живую сущность, которая берет на себя выполнение определенных задач, вместо "широких" классов нужно использовать много более конкретных.
```
*  Никита Сальников-Тарновский - Сколько занимают объекты Java в памяти. [ссылка](https://www.youtube.com/watch?v=raFDt883fFQ) **(6/10)**
```
Заголовок объекта (8 или 12 байт), выравнивание, хранение массивов, размер примитива и его обертки (Wrapper), заголовок устраняет неоднозначность в размере объектов, опасность использования коллекций (альтернатива TROOVE)
```
* Алексей Шипилёв — Сжимай меня полностью. [ссылка](https://www.youtube.com/watch?v=hOF7sewi6pk&t) **(10/10)**
```
Выравнивание, распределение данных по полям, cash miss, сжатые ссылки (4Гб< и >4Гб), влияние выравнивания на механизм адресации (режим сжатых ссылок), True/False Sharing (работа процессоров с cash lines, причина cash misses), Card table, сжатые String (в jdk8 еще нет, тип сжатия описывается в переменной)
```
* Никита Липский, Владимир Иванов — JVM: краткий курс общей анатомии. [ссылка](https://www.youtube.com/watch?v=-fcj6EL9rc4) **(6/10)**
```
пересмотреть
```
* Алексей Шипилёв — Катехизис java.lang.String. [ссылка](https://www.youtube.com/watch?v=SZFe3m1DV1A) **(5/10)**
```
пересмотреть
```
* Александр Маторин — Неадекватное Java-интервью. [ссылка](https://www.youtube.com/watch?v=AR9dtVaEUSM) **(7/10)**
```
Нельзя сравнивать объекты разных классов через "==", у StringBuilder не переопределен equals, приоритет выбора метода при перегрузке (расширение до примитивов -> боксинг -> var ags), размер кэша для Long не увеличивается через аргументы jvm, finally выполняется даже при StackOverflow etc, что при рекурсии может привести к зависанию программы. Фишка с a[--i] = 1/--i. Если в статическом блоке ошибка, то при повторном обращении NoClassDefError, при расширении интейрфейса в котором метод выкидает исключения, результирующий список исключений метода должен быть нерасширяющим, в перечислениях конструктор элементов выполняется до статического блока.
```
* Роман Елизаров — Теоретический минимум для понимания Java Memory Model. [ссылка](https://www.youtube.com/watch?v=hxIRyqHRnjE&feature=youtu.be) **(4/10)**
```
Линериализуемость (=атомарность) (для всего) и последовательная согласованность (для системы, но не для одного объекта). Вернуться к докладу после, сложная тема.
```
* Алексей Шипилёв — Прагматика Java Memory Model. [ссылка](https://www.youtube.com/watch?v=iB2N8aqwtxc&feature=youtu.be) **(8/10)**
```
Невыровненное чтение разрушает атомарность, word tearing (поэтому boolean min space = 1 bite (cash line size), а с bitset нельзя работать в нескольких потоках), long/double - в x32 не атомарны, syncronization order (спец.маркеры: volatile read/write,  lock/unlock монитора, 1-ое/последнее действие в потоке и команды по типу join(), isInterrupted() и т.п.), принцип happens before (read получает значение переменной выше по выше happens-before.
```
