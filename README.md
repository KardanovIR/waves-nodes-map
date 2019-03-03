#Waves Maps on the map

This project puts all known Waves Nodes to the map and shows their geo information.

[Demo](https://kardanovir.github.io/waves-nodes-map)

It grabs data about Waves Nodes in four steps:
1) Get all connected peers to the Waves Public Pool (`nodes.wavesplatform.com`) and store about the peers.
2) Try to get information about connected nodes from all nodes from the first step (it tries to request them by ports 80 and 6869, which is default for Waves Node REST API).
3) Merge all lists of peers to one list.
4) Using [geoiplookup.io](https://geoiplookup.io) gathers data about location of servers.

### Dependencies
- [Bootstrap](https://getbootstrap.com/) for design
- [JQuery](https://jquery.com/) for nostalgia
- [Bootstrap Table](https://bootstrap-table.com) because of laziness of the author
- [Yandex Maps](https://maps.yandex.ru) for maps