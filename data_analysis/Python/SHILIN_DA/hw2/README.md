ДЗшка 2 

Подробное задание в файле шаблона.
Максимально использовать Pandas и Plotly или Bokeh или GeoPandas (для визуализации карты Мира со странами). Применение излишних циклов ведет к снижению баллов (циклы ЗЛО). Применение ненужных функций аналогично. Используйте apply, mар и lambda по максимуму. Помним про корректное применение сортировок.
Вспоминаем английский:

csv_airports_v1.csv (данные по аэропортам):
- Airport ID Unique OpenFlights identifier for this airport.
- Name of airport. May or may not contain the City name.
- City Main city served by airport. May be spelled differently from Name.
- Country Country or territory where airport is located. See Countries to cross-reference to ISO 3166-1 codes.
- IATA 3-letter IATA code. Null if not assigned/unknown.
- ICAO 4-letter ICAO code. Null if not assigned.
- Latitude Decimal degrees, usually to six significant digits. Negative is South, positive is North.
- Longitude Decimal degrees, usually to six significant digits. Negative is West, positive is East. Altitude In feet.
- Timezone Hours offset from UTC. Fractional hours are expressed as decimals, eg. India is 5.5.
- DST Daylight savings time. One of E (Europe), A (US/Canada), S (South America), O (Australia), Z (New Zealand), N (None) or U (Unknown). See also: Help: Time
- Tz database timezone Timezone in "tz" (Olson) format, eg. "America/Los_Angeles".

csv_routes_v1.csv (данные по перелетам):
- Airline 2-letter (IATA) or 3-letter (ICAO) code of the airline.
- Airline ID Unique OpenFlights identifier for airline (see Airline).
- Source airport 3-letter (IATA) or 4-letter (ICAO) code of the source airport.
- Source airport ID Unique OpenFlights identifier for source airport (see Airport)
- Destination airport 3-letter (IATA) or 4-letter (ICAO) code of the destination airport.
- Destination airport ID Unique OpenFlights identifier for destination airport (see Airport)
- Equipment 3-letter codes for plane type(s) generally used on this flight, separated by spaces

Задания: 
1) Определить ТОП10 аэропортов по количеству вылетов и прилетов
2) Найти и показать ошибки (нелогичности) в датасетах
3) Для каждого материка отобразить ТОП5 аэропортов на карте при помощи маркеров,
и соединить все эти аэропорты ГЕОЛИНИЯМИ, причем, если можно вылететь из двух аэропортов в обе стороны,
то и стрелочка в обе стороны, а если только в одну сторону, то стрелочка в соответствующую сторону (визуализашка, лучше использовать библиотеку Plotly)
