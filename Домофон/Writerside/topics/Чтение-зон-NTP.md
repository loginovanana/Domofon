# Чтение зон NTP

Получить список доступных часовых зон для NTP.

## Формат запроса

| <format style="" color="Blue"> GET </format>     | URI: `http://{{panel_address}}/api/v1.cgi/network/ntp/zone` |
|--------------------------------------------------|-------------------------------------------------------------|

## Формат ответа

### <format style="" color="LawnGreen">200 OK</format> 

<tabs>
<tab title="JSON">

```JSON
[
 "DatelineStandardTime12",
 "<UTC-11>11",
 "AleutianStandardTime10DaylightTime,M3.2.0,M11.1.0",
 "HawaiianStandardTime10",
 "MarquesasStandardTime9:30",
 "AlaskanStandardTime9DaylightTime,M3.2.0,M11.1.0",
 "<UTC-09>9",
 "<UTC-08>8",
 "PacificStandardTimeMexico8DaylightTime,M3.2.0,M11.1.0",
 "PacificStandardTime8DaylightTime,M3.2.0,M11.1.0",
 "USMountainStandardTime7",
 "MountainStandardTime7DaylightTime,M3.2.0,M11.1.0",
 "YukonStandardTime7",
 "CentralStandardTimeMexico6",
 "EasterIslandStandardTime6DaylightTime,M9.1.6/22,M4.1.6/22",
 "CanadaCentralStandardTime6",
 "CentralAmericaStandardTime6",
 "CentralStandardTime6DaylightTime,M3.2.0,M11.1.0",
 "SAPacificStandardTime5",
 "EasternStandardTime5DaylightTime,M3.2.0,M11.1.0",
 "CubaStandardTime5DaylightTime,M3.2.0/0,M11.1.0/1",
 "HaitiStandardTime5DaylightTime,M3.2.0,M11.1.0",
 "USEasternStandardTime5DaylightTime,M3.2.0,M11.1.0",
 "TurksAndCaicosStandardTime5DaylightTime,M3.2.0,M11.1.0",
 "EasternStandardTimeMexico5",
 "ParaguayStandardTime4DaylightTime,M10.1.0/0,M3.4.0/0",
 "AtlanticStandardTime4DaylightTime,M3.2.0,M11.1.0",
 "SAWesternStandardTime4",
 "VenezuelaStandardTime4",
 "CentralBrazilianStandardTime4",
 "TocantinsStandardTime3",
 "ESouthAmericaStandardTime3",
 "ArgentinaStandardTime3",
 "SAEasternStandardTime3",
 "MontevideoStandardTime3",
 "MagallanesStandardTime3",
 "BahiaStandardTime3",
 "SaintPierreStandardTime3DaylightTime,M3.2.0,M11.1.0",
 "<UTC-02>2",
 "AzoresStandardTime1DaylightTime,M3.5.0/0,M10.5.0/1",
 "CapeVerdeStandardTime1",
 "UTC0",
 "GMTStandardTime0DaylightTime,M3.5.0/1,M10.5.0",
 "GreenwichStandardTime0",
 "SaoTomeStandardTime0",
 "MoroccoStandardTime0DaylightTime,M4.4.0,M3.3.0/3",
 "WEuropeStandardTime-1DaylightTime,M3.5.0,M10.5.0/3",
 "CentralEuropeStandardTime-1DaylightTime,M3.5.0,M10.5.0/3",
 "RomanceStandardTime-1DaylightTime,M3.5.0,M10.5.0/3",
 "CentralEuropeanStandardTime-1DaylightTime,M3.5.0,M10.5.0/3",
  "WCentralAfricaStandardTime-1",
  "GTBStandardTime-2DaylightTime,M3.5.0/3,M10.5.0/4",
  "FLEStandardTime-2DaylightTime,M3.5.0/3,M10.5.0/4",
  "NamibiaStandardTime-2",
  "SouthSudanStandardTime-2",
  "IsraelStandardTime-2DaylightTime,M3.4.5,M10.5.0",
  "KaliningradStandardTime-2",
  "EEuropeStandardTime-2DaylightTime,M3.5.0,M10.5.0/3",
  "LibyaStandardTime-2",
  "SouthAfricaStandardTime-2",
  "SudanStandardTime-2",
  "JordanStandardTime-3",
  "ArabicStandardTime-3",
  "VolgogradStandardTime-3",
  "ArabStandardTime-3",
  "BelarusStandardTime-3",
  "RussianStandardTime-3",
  "EAfricaStandardTime-3",
  "TurkeyStandardTime-3",
  "IranStandardTime-3:30",
  "ArabianStandardTime-4",
  "AstrakhanStandardTime-4",
  "AzerbaijanStandardTime-4",
  "CaucasusStandardTime-4",
  "<RussiaTimeZone3>-4",
  "MauritiusStandardTime-4",
  "SaratovStandardTime-4",
  "GeorgianStandardTime-4",
  "AfghanistanStandardTime-4:30",
  "WestAsiaStandardTime-5",
  "EkaterinburgStandardTime-5",
  "PakistanStandardTime-5",
  "QyzylordaStandardTime-5",
  "IndiaStandardTime-5:30",
  "SriLankaStandardTime-5:30",
  "NepalStandardTime-5:45",
  "CentralAsiaStandardTime-6",
  "BangladeshStandardTime-6",
  "OmskStandardTime-6",
  "MyanmarStandardTime-6:30",
  "SEAsiaStandardTime-7",
  "AltaiStandardTime-7",
  "NorthAsiaStandardTime-7",
  "NCentralAsiaStandardTime-7",
  "TomskStandardTime-7",
  "WMongoliaStandardTime-7",
  "ChinaStandardTime-8",
  "NorthAsiaEastStandardTime-8",
  "SingaporeStandardTime-8",
  "WAustraliaStandardTime-8",
  "TaipeiStandardTime-8",
  "UlaanbaatarStandardTime-8",
  "AusCentralWStandardTime-8:45",
  "TokyoStandardTime-9",
  "NorthKoreaStandardTime-9",
  "KoreaStandardTime-9",
  "TransbaikalStandardTime-9",
  "YakutskStandardTime-9",
  "AUSCentralStandardTime-9:30",
  "EAustraliaStandardTime-10",
  "VladivostokStandardTime-10",
  "WestPacificStandardTime-10",
  "AUSEasternStandardTime-10DaylightTime,M10.1.0,M4.1.0/3",
  "TasmaniaStandardTime-10DaylightTime,M10.1.0,M4.1.0/3",
  "MagadanStandardTime-11",
  "BougainvilleStandardTime-11",
  "SakhalinStandardTime-11",
  "CentralPacificStandardTime-11",
  "<RussiaTimeZone10>-11",
  "NorfolkStandardTime-11DaylightTime,M10.1.0,M4.1.0/3",
  "<RussiaTimeZone11>-12",
  "<UTC+12>-12",
  "FijiStandardTime-12",
  "NewZealandStandardTime-12DaylightTime,M9.5.0,M4.1.0/3",
  "TongaStandardTime-13",
  "<UTC+13>-13",
  "SamoaStandardTime-13DaylightTime,M9.5.0/3,M4.1.0/4",
  "LineIslandsStandardTime-14"
]
```
</tab>
</tabs>
<note>
В ответе представлен список часовых поясов.

Каждая строка в списке представляет часовой пояс и состоит из следующих элементов:

1. Название часового пояса: Например, “PacificStandardTime8DaylightTime”.
2. Смещение от UTC: Обычно это число с префиксом “+” или “-“, которое указывает на количество часов, на которое часовой пояс смещен от UTC. Например, “-8” означает, что часовой пояс отстает от UTC на 8 часов.
3. Дополнительные параметры (необязательно):
* DaylightTime: Указывает, что в этом часовом поясе действует летнее время.
* M3.2.0,M11.1.0: Это параметры перехода на летнее время DST (Daylight Saving Time).

    a) M: Означает “Март”, “Май”, “Июнь”, “Июль”, “Август”, “Сентябрь”, “Октябрь”, “Ноябрь”, “Декабрь”.

    b) Число: Указывает день месяца.

    c) Неделя: Необязательный параметр, указывающий номер недели месяца. Например, “M3.2.0/3” означает “Третья неделя марта, второй день”.
</note>

