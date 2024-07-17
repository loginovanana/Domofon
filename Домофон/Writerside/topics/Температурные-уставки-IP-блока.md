# Температурные уставки IP-блока

Управление температурными уставками для IP-блока.

## Чтение температурных уставок IP-блока {id="1"}

Получить информацию о текущих значениях температурных уставок.

### Формат запроса

| <format style="" color="Blue"> GET </format>     | URI: `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/ip_block` |
|--------------------------------------------------|----------------------------------------------------------------------|

### Формат ответа

###  <format style="" color="LawnGreen">200 OK</format> 

<tabs>
<tab title="JSON">

```JSON
{
  "iTemperatureHeatOff": -10,
  "iTemperatureHeatOn": -20,
  "iTemperatureIPBlockPowerOff": -15,
  "iTemperatureIPBlockPowerOn": -10
}
```
</tab>
</tabs>

| Атрибут                     | Описание                                               | Тип данных |
|-----------------------------|--------------------------------------------------------|------------|
| iTemperatureHeatOff         | Температура, при которой отключается отопление.        | integer    |
| iTemperatureHeatOn          | Температура, при которой включается отопление.         | integer    |
| iTemperatureIPBlockPowerOff | Температура, при которой отключается питание блока IP. | integer    |
| iTemperatureIPBlockPowerOn  | Температура, при которой включается питание блока IP.  | integer    |

## Редактирование температурных уставок IP-блока {id="2"}

Изменить значения температурных уставок.

### Формат запроса

| <format style="" color="ForestGreen"> POST </format> | URI: `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/ip_block` |
|------------------------------------------------------|----------------------------------------------------------------------|

### Тело запроса

<tabs>
<tab title="JSON">

```JSON
{
  "oGConfigIPBlock" : {
    "iTemperatureHeatOn" : -20,
    "iTemperatureHeatOff" : -10,
    "iTemperatureIPBlockPowerOn" : -10,
    "iTemperatureIPBlockPowerOff" : -15
  }
}
```
</tab>
</tabs>

| Атрибут                      | Описание                                               | Тип данных |
|------------------------------|--------------------------------------------------------|------------|
| oGConfigIPBlock              | Массив, представляющий температурные уставки IP-блока. | array      |
| iTemperatureHeatOff          | Температура, при которой отключается отопление.        | integer    |
| iTemperatureHeatOn           | Температура, при которой включается отопление.         | integer    |
| iTemperatureIPBlockPowerOff  | Температура, при которой отключается питание блока IP. | integer    |
| iTemperatureIPBlockPowerOn   | Температура, при которой включается питание блока IP.  | integer    |


### Коды ответа

| Код | Причина         | Описание                                 |
|-----|-----------------|------------------------------------------|
| 200 | OK              | Успешный ответ.                          |



