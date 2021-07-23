# Impermanent Loss

Wenn ein Farmer Liquitität bei einem AMM zur Verfügung stellt, werden die beiden Assets in einer 50:50 Ratio eingezahlt \(zum Zeitpunkt der Einzahlung\). Die Protokolle der AMM werden durch komplexe mathematische Formeln gesteuert, welche die Ratio der beiden zugrundeliegenden Token immer wieder anpasst und gleichzeitig deren Preis ermittelt. Weil der Wert von AVAX und ETH fluktuiert passt der AMM die Ratio des LP immer wieder an um eine Ratio von 50:50 zu erhalten. Das hat zur Folge dass Farmer an Einnahmen einbüßen sollte einer der beiden Token den anderen in der Performance übertreffen.

Nehmen wir für dieses Beispiel an 1 ETH = 100 AVAX & 100 AVAX = 1 ETH. Der Farmer stellt bei einem AMM Liquidität in Form von 100 AVAX und 1 ETH zur Verfügung und erhält dafür einen "Beleg" in Form von \(LP\) Token. Diese Token nutzt der Farmer um sie bei Yield Yak anzulegen. Sollte der Preis von AVAX steigen weil mehr und mehr Leute AVAX kaufen passt der AMM die Ratio im Pool an, sodass der Gesamtwert beider Token des Paares weiterhin einer Ratio von 50:50 entspricht.

Jetzt ist plötzlich 1 ETH nur mehr 50 AVAX wert weil der Preis von AVAX so sehr gestiegen ist. Weil das AMM Protokoll jedoch automatisch die Menge der Token im Pool angepasst hat, profitiert der Farmer von der Wertsteigerung nicht.

Dieses Verhalten wird als "Impermanent Loss" bezeichnet. Wenn sowohl der Preis von ETH wie auch der von AVAX gemeinsam in eine Richtung fluktuieren wird kein "Impermanent Loss" realisiert. Wenn hingegen der Wert nur eines der beiden Assets stark steigt profitiert der Farmer davon nicht.

Im Beispiel oben hätte der Farmer mehr Gewinn erzielt in dem er die Liquität aus dem pool entfernt und einfach nur die AVAX und ETH gehalten hätte.

Trotzdem ist anzumerken dass, wenn der Farmer seine Liquität im Pool behält, und der Preis von AVAX sinkt wieder zum ursprünglichen Wert, entsprechen auch die LP Tokens des Farmer wieder den ursprünglichen 100 AVAX und 1 ETH \(oder sogar mehr wenn der Farmer Yield Yak verwendet!\).

![](../../.gitbook/assets/il-graph.png)

Behalte im Kopf, Impermanent Losses werden nur dann zu permanenten Verlusten wenn du die Liquidität aus dem Pool entfernst.

## Wie kann man sich vor Impermanent Loss schützen?

Ein Weg sich vor Impermanent Loss zu schützen ist Liquiditäts-Paare zu wählen bei denen der Preis beider Assets relativ konstant ist. Zum Beispiel  exponiert man sich mit einem "Stablecoin"-Paar wie DAI-USDT dem IL Risiko so gut wie gar nicht.

Der Nachteil dieser Pools ist allerdings dass man von Preissteigerungen nicht profitiert, sie selten sind und der Ertrag meist niedriger ist als bei anderen Pools.

