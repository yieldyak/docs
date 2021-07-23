# Der Reinvestieren Button

## Muss ich den Reinvestieren Button betätigen?

Nein. Jemand anders wird den Button betätigen und du erhältst deine Belohnung.

## Wie funktioniert das?

Der Reinvestieren Button nimmt sich alle Belohungen des Pool, konvertiert sie in das Asset der Farm und Reinvestiert es zurück in den Pool um die Anlagen aller Nutzer der Farm zu vermehren.

Für jede Farm ist eine in der Höhe variable Belohnung für das Reinvestieren definiert. Wer als erstes den Button betätigt, erhält diese Belohnung und vermehrt die Anlagen aller Nutzer des Pool.

## Wann soll ich den Button betätigen?

Der Reinvestieren Button ist optional. Du musst den Button nicht betätigen. Manchmal macht es jedoch Sinn den Button zu drücken um die Belohnung zu kassieren.

Wenn es dein Ziel ist durch die Betätigung des Button einen Profit in AVAX zu generieren musst du das Belohnungs-Token / AVAX Preis Verhältnis, die Kosten für die Betätigung des Reinvestieren Button, die Kosten um die Belohnung in AVAX zu konvertieren etc. im Blick behalten und diese Kosten, der Belohnung für die Betätigung gegenüberstellen.

Um den Reinvestieren Button betätigen zu dürfen musst du keine Anlagen in der jeweiligen Farm haben. Jeder kann den Button betätigen und bekommt dafür die Belohnung. Behalte das im Hinterkopf wenn du vorhast den Button zu betätigen den es gibt viel Konkurrenz und du musst schnell sein.

## Beispiel einer Reinvestition

Nehmen wir an du hast Anlagen im folgendem Pool \(Pangolin ETH-AVAX / PEFI\)

![](../.gitbook/assets/screen-shot-2021-05-14-at-9.06.18-pm.png)

Um Teil dieses Pools zu sein hast du Liquidität in Form von ETH und AVAX auf Pangolin zu Verfügung gestellt und hast deine LP Token in der Yield Yak Farm angelegt. Diese LP Token wiederum werden dann von Yield Yak auf Penguin Finance in der entsprechenden Farm angelegt welche Belohnungen in Form von PEFI Tokens ausbezahlt. 

Ein Nutzer betätigt den Reinvestieren Button wenn die Menge der Belohnungen für die Yield Yak Farm 100 PEFI beträgt.

* Der Nutzer erhält für das Betätigen des Button 3 PEFI \(vorausgesetzt die Farm hat 3% Belohnung\)
* Yield Yak behält 5 PEFI als Rücklagen ein \(vorausgesetzt die Farm hat eine Gebühr von 5%\)
* Die übrigen PEFI werden reinvestiert

Die übrigen PEFI werden für ETH und AVAX verkauft, als Liquitität auf Pangolin hinterlegt und die LP Token wieder im Pool angelegt.

## Weitere Informationen

### Schutzmechanismen

Die Reinvestieren Funktion beinhaltet einen Schutzmechanismus welcher die Zeitspanne zwischen zwei Reinvestitionen reguliert. Durch den Schutzmechanismus sollte die zweite Transaktion \(welche fast keine Belohnung erhalten würde\) fehlschlagen und dadurch weniger Gas zahlen \(~0,03 AVAX\) anstatt den vollen Preis der Transaktion übernehmen zu müssen.

Solltest du entdecken dass eine Transaktion trotz des Schutzmechanismus nicht fehlschlägt und du nur eine sehr geringe Belohnung erhältst, melde dies bitte dem Team welches dann die Konfiguration der Farm anpasst.

### Transaktion fehlgeschlagen

Falls die Transaktion einer Reinvestition fehlschlägt ist dies auf Grund der folgenden zwei Gründe normal:

1. Du hast es wie oben geschafft das die Transaktion durchgeht obwohl die minimale Belohnung noch nicht erreicht wurde. Du zahlt jedoch nur einen Bruchteil der Transaktionskosten \(~0,03 AVAX\)
2. Aus irgendeinem Grund ist das Standard Gas Limit für die Transaktion nicht ausreichend. Eventuell musst du manuell das Gas Limit erhöhen. Schlägt die Transaktion deshalb fehl, kostet dich dies eventuell das gesamte Standard Gas Limit.

### Gebühren

Jedes mal wenn in eine Farm Reinvestiert werden Gebühren fällig.

Die Gebühren betragen meistens zwischen 5-10% der Belohnungen. Die Gebühren sind variable und ändern sich je nach Status des Netzwerk und um die Erträge der Farm zu optimieren. Es gibt drei Kategorien von Gebühren:

1. **Reinvestitionsgebühr** - Wird an den Nutzer der die Reinvestition durchführt ausbezahlt
2. **Admin Gebühr** - Wird an das Netzwerk ausbezahlt
3. **Entwickler Gebühr** - Wird an den Entwickler der die Strategie programmiert hat ausbezahlt

Yield Yak bezieht keine Gebühren für eine Einzahlung oder Auszahlung \(die zugrundeliegende Farm vielleicht jedoch schon\).

