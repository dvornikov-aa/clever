Мобильный пульт
===

Возможно управлять квадрокоптером в мобильного пульта через Wi-Fi. Он разработан в виде приложения для iOS и Android (TODO). Также существует упрощенная версия в виде [веб-страницы](#веб-версия).

![](assets/IMG_4397.PNG)

> **Warning** Мобильный пульт предназначен в первую очередь для полетов в помещении на дальность не более 10-15 м. Большое количество Wi-Fi сетей также может ухудшить отзывчивость и дальность пульта.

Для включения бэкенда пульта, установите [образ Clever на RPi](microsd_images.md), а также убедитесь, что он включен в launch-файле Клевера (`~/catkin_ws/src/clever/clever/launch/clever.launch`):

```xml
<arg name="rc" value="true"/>
```

При изменении launch-файла необходимо перезапустить пакет `clever`:

```bash
sudo systemctl restart clever
```

Также необходимо убедиться, что PX4-параметр `COM_RC_IN_MODE` установлен в значение `0` (RC Transmitter).

> **Note** Мобильный пульт конфликтует с реальной аппаратурой радиоуправления. Во время использования мобильного пульта она должны быть выключена.

Для управления коптером установите приложение на смартфон, подключитесь с Wi-Fi сети Клевера (`CLEVER-xxxx`), затем запустите приложение.

Стики на экране приложения работают также, как и реальные стики. Для арминга коптера подержите левый стик в правом нижнем углу на протяжении нескольких секунд. Для дизарминга – в левом нижнем углу.

Пульт отображает текущий [режим PX4](modes.md) а также уровень заряда батареи. При низком значении заряда батареи телефон будет вибрировать.

> **Note** Если интерфейс пульта отображает явно неправильное напряжение (напр. > 5 V), проверьте, что значение PX4-параметра `BAT_N_CELLS` соответствует реальному количество элементов батареи. Если отображаемое напряжение все равно неверно, откалибруйте батарею (TODO: ссылка).

> **Note** Если вместо режима PX4 отображается текст "DISCONNECTED FROM FCU", проверьте [подключение Raspberry Pi к PixHawk](connection.md).

Веб-версия
---

TODO