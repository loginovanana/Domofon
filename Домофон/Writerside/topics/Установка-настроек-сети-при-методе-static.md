# Метод static

“Static” означает, что IP-адрес устройства назначается вручную, а не автоматически через DHCP-сервер.

## Чтение настроек сети при методе static {id="1"}

Получить информацию о статических настройках сети устройства.

### Формат запроса

| <format style="" color="Blue"> GET </format>     | URI: `http://{{panel_address}}/api/v1.cgi/network/lan/static` |
|--------------------------------------------------|---------------------------------------------------------------|

### Формат ответа

###  <format style="" color="LawnGreen">200 OK</format> 

<tabs>
<tab title="JSON">  

```JSON
{
  "sDNS1": "192.168.251.62",
  "sDNS2": "8.8.8.8",
  "sV4Address": "172.24.1.50",
  "sV4Gateway": "172.24.1.49",
  "sV4Netmask": "255.255.255.240"
}
```
</tab>
</tabs>



| Атрибут    | Описание                                                      | Тип данных |
|------------|---------------------------------------------------------------|------------|
| sDNS1      | Содержит IP-адрес первого DNS-сервера.                        | string     |
| sDNS2      | Содержит IP-адрес второго DNS-сервера.                        | string     |
| sV4Address | Содержит IP-адрес устройства в формате IPv4.                  | string     |
| sV4Netmask | Содержит  маску подсети в формате IPv4.                       | string     |
| sV4Gateway | Содержит информацию о IP-адресе шлюза LoRaWAN в формате IPv4. | string     |


## Установка настроек сети при методе static {id="2"}

Изменить статические настройки сети устройства.

### Формат запроса

| <format style="" color="ForestGreen"> POST </format> | URI: `http://{{panel_address}}/api/v1.cgi/network/lan/static` |
|------------------------------------------------------|---------------------------------------------------------------|

### Тело запроса

<tabs>
<tab title="JSON">

```JSON
{
  "sDNS1" : "8.8.8.8",
  "sDNS2" : "10.22.12.1",
  "sV4Address" : "172.16.16.197",
  "sV4Netmask" : "255.255.255.0",
  "sV4Gateway" : "10.22.12.1"
}
```
</tab>
</tabs>

| Атрибут    | Описание                                                      | Тип данных |
|------------|---------------------------------------------------------------|------------|
| sDNS1      | Содержит IP-адрес первого DNS-сервера.                        | string     |
| sDNS2      | Содержит IP-адрес второго DNS-сервера.                        | string     |
| sV4Address | Содержит IP-адрес устройства в формате IPv4.                  | string     |
| sV4Netmask | Содержит  маску подсети в формате IPv4.                       | string     |
| sV4Gateway | Содержит информацию о IP-адресе шлюза LoRaWAN в формате IPv4. | string     |


## Коды ответа

| Код | Причина          | Описание                                                  |
|-----|------------------|-----------------------------------------------------------|
| 200 | OK               | Успешный ответ.                                           |