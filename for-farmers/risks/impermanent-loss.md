# Impermanent Loss

Lorsqu'un agriculteur fournit des liquidités sur un AMM, les deux actifs sont déposés à un ratio de 50:50 de leur valeur l'un par rapport à l'autre \(au moment du dépôt\). Les protocoles des AMM sont contrôlés par des formules mathématiques complexes qui ajustent les ratios des actifs sous-jacents dans le pool tout en déterminant également leurs prix. Comme la valeur de l'AVAX et de l'ETH fluctue, l'AMM ajustera le ratio des fermiers LP pour s'assurer qu'ils restent à une valeur de 50:50. Cela signifie qu'un fermier peut perdre les gains d'un actif déposé qui surperforme.

Ainsi, pour les besoins de cet exemple, supposons que 1 ETH = 100 AVAX et 100 AVAX = 1 ETH. l'utilisateur fournit des liquidités sur un AMM et dépose 100 AVAX et 1 ETH et reçoit le jeton de "réception" \(LP\) qui peut ensuite être déposé sur Yield Yak pour s'auto-composer. Dans le cas où le prix de l'AVAX commence à augmenter car de plus en plus de personnes achètent de l'AVAX. Dans ce cas, la pool ajuste le ratio pour s'assurer que la valeur reste répartie à 50:50 entre AVAX et ETH.

Maintenant, 1 ETH ne vaut soudainement plus que 50 AVAX à cause de la hausse du prix des AVAX. Mais comme le protocole a automatiquement ajusté la quantité de jetons dans le pool, l'utilisateur a perdu sur la hausse de l'AVAX.

C'est une perte impermanente. Si les prix de l'ETH et de l'AVAX fluctuent en ligne l'un avec l'autre, alors aucune IL n'est réalisée. Mais si le prix de l'un des deux actifs augmente considérablement, l'utilisateur est perdant.

Dans l'exemple ci-dessus, l'utilisateur aurait mieux fait de simplement hodler ses AVAX/ETH s'il avait retiré ses liquidités du pool de l'AMM.

Cependant, si l'utilisateur reste dans la pool et que la valeur de l'AVAX revient à sa valeur initiale, la valeur de l'ensemble de ses avoirs reviendra également à sa valeur initiale et il aura 100 AVAX et 1 ETH \(ou même plus s'il a déposé ses jetons LP sur Yield Yak !\)  


![](../../.gitbook/assets/il-graph.png)

N'oubliez pas que les pertes impermanentes ne deviennent permanentes que lorsque vous retirez vos liquidités.

## Comment se protéger contre l’IL ?

Une façon de réduire votre exposition à l'IL est de fournir des liquidités pour des paires où le prix relatif de chaque actif reste relativement constant. Par exemple, une paire de monnaies stables comme DAI-USDT vous exposerait très peu à l'IL.

Cependant, l'inconvénient de ces pools est que vous ne bénéficiez pas de l'augmentation des prix, que le nombre de ces pools est réduit et que les rendements peuvent ne pas être aussi intéressants que ceux d'autres pools.

