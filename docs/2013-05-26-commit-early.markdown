---
layout: post
title: "Commit Early, Commit Often"
date: 2013-05-26 12:51
comments: true
published: false
categories: 
---
Draft nach mail von Dirk:
* zum Thema "commit early commit often" und "die richtige Größe für
Commits" gefällt mir bei Git sehr gut, dass man (lokal) die History
ändern kann; dadurch ergibt sich bei mir in der Regel folgender Workflow:

1) wirklich oft committen (eigentlich nach jeder nicht trivialen
Änderung bzw. vor jeder Entscheidung bei der ich mir noch nicht sicher
bin, ob es der richtige Weg ist) - ich committe hier zwischendurch auch
unrelated changes (Tippfehler in Kommentaren, etc.), aber jeweils in
einem eigenen, abgeschlossenen Commit

2) vor einem Push bzw. vor dem nächsten Merge räume ich die letzten
Commits nochmal auf (mittels "git rebase -i") :

* umsortieren der Commits
* zusammenfassen von zu kleinen Commits bzw. aufbrechen von Commits, die unrelated Changes enthalten
* ordentliches Ausformulieren der Commit-Messages

Der Vorteil dieser Methode ist, dass die History nachher schön
aufgeräumt (und damit gut durchsuchbar) ist und dass man trotzdem
während der Entwicklung jederzeit "Sicherheitssnapshots" machen kann