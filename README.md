# Что это?

Этот проект каждые 6 часов автоматически генерирует GeoSite файлы, в которые включены списки заблокированных Роскомнадзором доменов для различного рода маршрутизаторов трафика и Proxy/VPN приложений.

Данные о блокировках роскомнадзора получаются из следующих источников:
- [antifilter.download](https://antifilter.download/)
- [community.antifilter.download](https://community.antifilter.download/)
- [re:filter](https://github.com/1andrevich/Re-filter-lists)

Дополнительно используются:
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community/tree/master/data) - огромный список доменов, разбитых по множеству сервисов, компаний и категорий.
- [AdGuard Dns Filter](https://github.com/AdguardTeam/AdguardSDNSFilter) - список рекламных доменов
- [Peter Lowe’s list](https://pgl.yoyo.org/adservers/serverlist.php) - список рекламных доменов
- [WindowsSpyBlocker](https://github.com/crazy-max/WindowsSpyBlocker) - список доменов, используемых windows (в том числе для слежки и сбора аналитики)

В списки так же загружаются дополнительные домены из [@runetfreedom/russia-domains-list](https://github.com/runetfreedom/russia-domains-list). Если хотите предложить какие-то домены или категории, то сделайте это там.


## Доступные категории

- Все категории из [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community/tree/master/data). Включая: google, discord, youtube, twitter, meta, openai и так далее.
- `geosite:ru-blocked` - заблокированные в России домены (`antifilter-download-community` + `re:filter`)
- `geosite:ru-blocked-all` - **все известные** заблокированные в России домены (`antifilter-download` + `antifilter-download-community` + `re:filter`). Список содержит не менее 700 тысяч доменов, употреблять с осторожностью.
- `geosite:ru-available-only-inside` - Домены, доступные только внутри России 
- `geosite:antifilter-download` - все домены из `antifilter.download` (почти 700 тысяч, употреблять с осторожностью)
- `geosite:antifilter-download-community` - все домены из `community.antifilter.download`
- `geosite:refilter` - все домены из `re:filter`
- `geosite:category-ads-all` - все рекламные домены
- `geosite:win-spy` - домены, используемые windows для слежки и сбора аналитики
- `geosite:win-update` - домены, используемые windows для обновлений
- `geosite:win-extra` - прочие домены, используемые windows

Релиз так же содержит эти категории в виде текстовых файлов со списком доменов.

# Cкачать

По ссылкам ниже всегда доступна последняя версия файлов.

- **github**
    - [https://raw.githubusercontent.com/runetfreedom/russia-blocked-geosite/release/geosite.dat](https://raw.githubusercontent.com/runetfreedom/russia-blocked-geosite/release/geosite.dat)
    - Hashsum: [https://raw.githubusercontent.com/runetfreedom/russia-blocked-geosite/release/geosite.dat.sha256sum](https://raw.githubusercontent.com/runetfreedom/russia-blocked-geosite/release/geosite.dat.sha256sum)
- **JSDelivr**
    - [https://cdn.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat](https://cdn.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat)
    - Hashsum: [https://cdn.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat.sha256sum](https://cdn.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat.sha256sum)
- **Fastly + JSDelivr**
    - [https://fastly.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat](https://fastly.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat)
    - Hashsum: [https://fastly.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat.sha256sum](https://fastly.jsdelivr.net/gh/runetfreedom/russia-blocked-geosite@release/geosite.dat.sha256sum)


## Смежные проекты

- [@runetfreedom/russia-blocked-geoip](https://github.com/runetfreedom/russia-blocked-geoip) - GeoIP файлы с заблокированными в России сетями и адресами
- [@runetfreedom/russia-v2ray-rules-dat](https://github.com/runetfreedom/russia-v2ray-rules-dat) - Правила для V2Ray, основанные на этих данных

## Благодарности

- [antifilter.download](https://antifilter.download/) - за предоставление данных о заблокированных доменах и комьюнити для их обновления
- [re:filter](https://github.com/1andrevich/Re-filter-lists) - за предоставление отфильтрованных данных о заблокированных доменах
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) - за идею и основу этого проекта