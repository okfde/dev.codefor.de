---
layout: project
lab: [dresden] #needed for Aggregation on Lab-Page
imgname: dresden/parkhaeuser-web.png
title: Freie Parkplätze Dresden

links:
- url: https://parkendd.de/map.html
  name: Karte (aktuelle Belegung)
- url: https://play.google.com/store/apps/details?id=de.jkliemann.parkendd
  name: ParkenDD Android App
- url: https://apps.apple.com/de/app/parkendd/id957165041
  name: ParkenDD iOS App
- url: https://mechlab-engineering.de/2015/03/vorhersage-der-parkhausbelegung-mit-offenen-daten/
  name: Vorhersage der Belegung mit Machine Learning


collaborators:
- name: Consti
  links:
  - url: https://twitter.com/ubahnverleih
    name: twitter
- name: rob
  links:
  - url: https://twitter.com/robtranquillo
    name: twitter
- name: jklmnn
  links:
  - url: https://twitter.com/JK70523
    name: twitter
- name: kiliankoe
  links:
  - url: https://twitter.com/kiliankoe
    name: twitter
- name: balzer82
  links:
  - url: https://twitter.com/balzer82
    name: twitter

tags:
- Mobilität

---

Die Stadt Dresden bietet auf [https://www.dresden.de/freie-parkplaetze](https://www.dresden.de/freie-parkplaetze) eine Übersicht der freien Parkplätze in der Stadt Dresden an. Leider nicht maschinenlesbar (barrierefrei). Darum haben wir uns gekümmert!
Die Daten werden in regelmäßigen Abständen von der Website geholt (gescraped) und in einer Datenbank gespeichert. Es wird eine [maschinenlesbare Schnittstelle (API)](https://github.com/offenesdresden/ParkAPI) bereitgestellt. Die historischen Daten wurden [analysiert und grafisch aufbereitet](https://mechlab-engineering.de/2015/03/vorhersage-der-parkhausbelegung-mit-offenen-daten/). Weiterhin wurde mittels Machine Learning ein Vorhersagemodell entworfen, welches es ermöglicht die Belegung eines Parkhauses in Zukunft vorherzusagen

![DataFlow](https://mechlab-engineering.de/wordpress/wp-content/uploads/2015/03/DataFlow.png)

Dies ist hilfreich für Veranstaltungsplanung oder Tourismus. Folgende Anwendungsfälle sind denkbar:

* Verkehrsleitung und Minimierung von Parkplatzsuchverkehren im Innenstadtbereich
* Touristen aus Tschechien können schon auf der Autobahn via App schauen, ob das anzusteuernde Parkhaus belegt sein wird
* Familien können vor dem Start in die Stadt schauen, ob Parkhaus dann (wenn die Kinder endlich angezogen und startklar sind) belegt sein wird und ÖPNV nicht die bessere Wahl wäre
* Veranstaltungsplanung kann schauen, wieviel Kapazität in 4 Monaten Samstag in den Parkhäusern zur Verfügung steht und ob ggf. extra Parkflächen nötig sind

![iOS App](https://parkendd.de/media/ios_frame.png)