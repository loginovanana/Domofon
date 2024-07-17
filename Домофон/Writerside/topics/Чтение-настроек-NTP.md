# Чтение настроек NTP

Получить информацию о текущих настройках NTP (Network Time Protocol) на устройстве.

## Формат запроса

| <format style="" color="Blue"> GET </format>     | URI: `http://{{panel_address}}/api/v1.cgi/network/ntp` |
|--------------------------------------------------|--------------------------------------------------------|

## Формат ответа

### <format style="" color="LawnGreen">200 OK</format> 
<tabs>
<tab title="JSON">

```JSON
{
 "bDstEnabled": false,
 "bNtpEnabled": true,
 "iRefreshTime": 60,
 "sNtpServers": "ntp0.ntp-servers.net ntp1.ntp-servers.net ntp2.ntp-servers.net 0.ru.pool.ntp.org 1.ru.pool.ntp.org 2.ru.pool.ntp.org",
 "sTimeZone": "RussianStandardTime-3"
}

```
</tab>
</tabs>

| Атрибут      | Описание                                                                     | Тип данных |
|--------------|------------------------------------------------------------------------------|------------|
| bDstEnabled  | Включение перехода на летнее время.                                          | boolean    |
| bNtpEnabled  | Включение синхронизации с ntp.                                               | boolean    |
| iRefreshTime | Интервал синхронизации с ntp сервером, в минутах.                            | integer    |
| sNtpServers  | Адреса ntp серверов, без указания портов. Только адрес или IP, через пробел. | string     |
| sTimeZone    | Имя временной зоны (список зон можно получить в отдельном запросе).          | string     |
