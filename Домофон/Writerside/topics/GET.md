# GET

В таблице ниже приведен список ресурсов API : 

| URI                                                                       | Название                                                                                     | 
| ------------------------------------------------------------------------- |----------------------------------------------------------------------------------------------|
| `http://{{panel_address}}/api/v1.cgi/system/device-info`                  | [](Чтение-информации-о-домофоне.md)                                                          |
| `http://{{panel_address}}/api/v1.cgi/system/time`                         | [](Чтение-системного-времени.md)                                                             | 
| `http://{{panel_address}}/api/v1.cgi/system/syslog/settings`              | [](Чтение-настроек-syslog.md)                                                                | 
| `http://{{panel_address}}/api/v1.cgi/intercom/snapshot`                   | [](Получение-моментального-снимка-с-камеры.md)                                               | 
| `http://{{panel_address}}/api/v1.cgi/intercom/appartments/<flat_id>`      | [](Чтение-данных-одной-квартиры.md)                                                          |        
| `http://{{panel_address}}/api/v1.cgi/intercom/appartments`                | [](Чтение-данных-всех-квартир.md )                                                           | 
| `http://{{panel_address}}/api/v1.cgi/intercom/rfids`                      | [](Чтение-данных-всех-RFID-ключей.md)                                                        | 
| `http://{{panel_address}}/api/v1.cgi/intercom/rfids/<key_uid>`            | [](Чтение-данных-одного-RFID-ключа.md)                                                       |                          
| `http://{{panel_address}}/api/v1.cgi/intercom/codes`                      | [](Чтение-данных-всех-кодов.md)                                                              |       
| `http://{{panel_address}}/api/v1.cgi/intercom/codes/<code_id>`            | [](Чтение-данных-одного-кода.md)                                                             |                                                                                                  
| `http://{{panel_address}}/api/v1.cgi/intercom/doors`                      | [](Чтение-состояния-всех-дверей.md)                                                          |                                                               
| `http://{{panel_address}}/api/v1.cgi/intercom/doors/<doors_id>`           | [](Чтение-состояния-одной-двери.md)                                                          |                                                                                                 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig`                    | [](Чтение-всех-конфигурационных-параметров.md)                                               |                                                          
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/info`               | [](Чтение-заголовка-набора-конфигурационных-параметров.md)                                   |  
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/timeouts`           | [Чтение таймаутов](Таймауты.md)                                                              | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/volume`             | [Чтение настроек громкости](Настройки-громкости.md)                                          | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/special_modes`      | [Чтение состояния специальных режимов](Специальные-режимы.md)                                | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/line_state_levels`  | [Чтение пороговых уровней напряжения в линии](Пороговые-уровни-напряжения-в-линии.md)        | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/default_codes`      | [Чтение сервисных кодов](Сервисные-коды.md)                                                  | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/ip_block`           | [Чтение температурных уставок IP-блока ](Температурные-уставки-IP-блока.md)                  | 
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/dtmf_codes`         | [Чтение кодов DTMF](Коды-DTMF.md)                                                            |                                                                                                             
| `http://{{panel_address}}/api/v1.cgi/intercom/gconfig/text`               | [Чтение текстовых сообщений](Текстовые-сообщения.md)                                         |                                                                                              
| `http://{{panel_address}}/api/v1.cgi/emergency_alert/volume`              | [](Чтение-настроек-громкости.md)                                                             |                                                                                                                    
| `http://{{panel_address}}/api/v1.cgi/intercom/sip/config`                 | [Чтение настроек SIP](SIP.md)                                                                |                                                                                                               
| `http://{{panel_address}}/api/v1.cgi/firmware/version`                    | [](Чтение-версий-прошивок.md)                                                                |                                                                                                                                                    
| `http://{{panel_address}}/api/v1.cgi/firmware/mcu/version`                | [](Чтение-версий-прошивок-Artery.md)                                                         |                                                                                                                                                    
| `http://{{panel_address}}/api/v1.cgi/firmware/cpu/version`                | [](Чтение-версии-прошивки-RockChip.md)                                                       |                                                                                                                                                     
| `http://{{panel_address}}/api/v1.cgi/firmware/mcu/update/state`           | [](Чтение-состояния-обновления-прошивки.md)                                                  |                                                                                                                                                   
| `http://{{panel_address}}/api/v1.cgi/network/ntp`                         | [](Чтение-настроек-NTP.md)                                                                   |                                                                                                                 
| `http://{{panel_address}}/api/v1.cgi/network/ntp/zone`                    | [](Чтение-зон-NTP.md)                                                                        |                                                                                                                                                    
| `http://{{panel_address}}/api/v1.cgi/network/lan`                         | [](Чтение-всех-общих-настроек-сети.md)                                                       |                                                                       
| `http://{{panel_address}}/api/v1.cgi/network/lan/method`                  | [](Чтение-метода-получения-адреса.md)                                                        |                                                                                                                      
| `http://{{panel_address}}/api/v1.cgi/network/lan/static`                  | [Чтение настроек сети при методе static](Установка-настроек-сети-при-методе-static.md)       |                               
| `http://{{panel_address}}/api/v1.cgi/network/lan/static/ip`               | [Чтение данных IP-адреса/маски при методе static](Чтение-настроек-сети-при-методе-static.md) |                                                
| `http://{{panel_address}}/api/v1.cgi/network/lan/static/dns`              | [Чтение настроек DNS](Настройки-DNS.md)                                                      |                                                                    
| `http://{{panel_address}}/api/v1.cgi/network/lan/static/gateway`          | [Чтение адреса шлюза](Адрес-шлюза.md)                                                        | 
| `http://{{panel_address}}/api/v1.cgi/intercom/dtmf/method`                | [Чтение метода DTMF](DTMF.md)                                                                | 

