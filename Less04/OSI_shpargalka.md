

Чтобы запомнить порядок уровней (с 1-го по 7-й) придумала такую фразу: PeDaNT SPA

И это действительно помогло, ведь сейчас шпаргалку я пишу по памяти:

* P - Physical (физический) - 1
* D - Data link (канальный) - 2
* N - Network (сетевой) - 3
* T - Transport (транспортный) - 4
* S - Session (сеансовый) - 5
* P - Presentation (представления) - 6
* A - Application (прикладной/приложений) - 7

Исходящий сигнал проходит процедуру инкапсуляции (проходит с 7 по 1 уровень), а у получателя сигнал проходит обратную процедуру - декапсуляция (проходит с 1 по 7 уровень).

И 4-й уровень связывает 3 уровня, относящихся к "сетевым железкам и проводам" (1, 2, 3) и 3 уровня "пользовательских" (5, 6, 7).
