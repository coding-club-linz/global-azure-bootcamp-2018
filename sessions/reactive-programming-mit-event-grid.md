---
layout: session
page-category: session
title: Reactive Programming mit Event Grid
speaker: Christoph Wille
speaker-id: christoph-wille
room: '15.04'
slot: 4
---

In modernen Lösungen sind Events überall - und obwohl Events so wichtig sind, muß man sehr viel Aufwand betreiben bevor man produktiv werden kann: das "plumbing" steht im Weg. Wie wäre es mit einer Lösung die das ganze Event Routing vom Publisher zum Subscriber übernehmen könnte? Inklusive Registrierung, Retry Logik, Monitoring, Delivery nahe Echtzeit und das ganze als Plattform Service der dynamisch skaliert? 
 
Azure Event Grid bietet all das und wird mittlerweile - obwohl ein sehr "junger" Service - innerhalb von Azure bereits von einigen Services als Publisher bedient. Für viele Szenarien wird damit das Programmieren von "hammer polling" beziehungsweise "exponential backoff" überflüssig, was im Endeffekt Geld spart (Rechenzeit, Transkationen) - und das ist bei Cloud Lösungen ein gewichtiges Argument. Event Grid ist aber nicht auf Events von Azure selbst beschränkt: es ist auch für die eigene Applikation als Event backbone geeignet - WebHook Subscription Management ade, willkommen push-push!