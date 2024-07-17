# Чтение данных всех RFID ключей

Получить информацию о всех RFID-ключах, зарегистрированных в системе.

## Формат запроса

| <format style="" color="Blue"> GET </format>     | URI: `http://{{panel_address}}/api/v1.cgi/intercom/rfids` |
|--------------------------------------------------|-----------------------------------------------------------|

## Формат ответа

### <format style="" color="LawnGreen">200 OK</format> 

<tabs>
<tab title="JSON">


```JSON
{
"iFlatID": 0,
"iKeyType": 0,
"iLockAccess": 0,
"iSceneID": 0,
"sKeyUid": "fc125589"
},
{
"iFlatID": 22,
"iKeyType": 0,
"iLockAccess": 0,
"iSceneID": 0,
"sKeyUid": "ab752589"
},
{
"iFlatID": 3,
"iKeyType": 0,
"iLockAccess": 0,
"iSceneID": 0,
"sKeyUid": "2345acfc"
}
```
</tab>
</tabs>

| Атрибут     | Описание                                                                                | Тип данных |
|-------------|-----------------------------------------------------------------------------------------|------------|
| iFlatID     | Указывает на номер квартиры, к которой привязан ключ.                                   | integer    |
| iKeyType    | Указывает на тип ключа (RFID ключ).                                                     | integer    |
| iLockAccess | Определяет, какие двери или зоны в здании можно открыть этим ключом.                    | integer    |
| iSceneID    | Указывает на конкретный режим в квартире, который активируется при использовании ключа. | integer    |
| sKeyUid     | Уникальный идентификатор RFID ключа.                                                    | string     |
