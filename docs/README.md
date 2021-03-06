Клевер
======

<img src="assets/clever3.png" align="right" width="300px" alt="Клевер">

«Клевер» — это учебный конструктор программируемого квадрокоптера, состоящего из популярных открытых компонентов, а также набор необходимой документации и библиотек для работы с ним.

Набор включает в себя полетный контроллер PixHawk/PixRacer с полетным стеком PX4, Raspberry Pi 3 в качестве управлящего бортового компьютера, модуль камеры для реализации полетов с использованием компьютерного зрения, а также набор различных датчиков и другой периферии.

На базе точно такой же платформы были созданы многие «большие» проекты компании Copter Express, например, дроны для [пиар-акций по автономной доставке пиццы](https://www.youtube.com/watch?v=hmkAoZOtF58) (Самара, Казань); дрон-доставщик кофе в Сколково, мониторинговый дрон с зарядной станцией, дроны-победители на полевых испытаниях «[Робокросс-2016](https://www.youtube.com/watch?v=dGbDaz_VmYU)», «[Робокросс-2017](https://youtu.be/AQnd2CRczbQ)» и многие другие.

Для того, чтобы научиться собирать, настраивать, пилотировать и программировать автономный дрон «Клевер», воспользуйтесь этим учебником.

Образ для Raspberry Pi
----------------------

**Образ ОС** для RPi 3 с предустановленным и преднастроенным ПО можно скачать [здесь](microsd_images.html).

Образ включает в себя:

* Raspbian Stretch
* ROS Kinetic
* Настроенную работу с сетью
* OpenCV
* mavros
* Набор ПО для работы с Клевером

[Описание API](simple_offboard.html) для автономных полетов.

Исходный код сборщика образа и всего ПО можно найти на [GitHub](https://github.com/CopterExpress/clever).
