# El Botón Reinvertir

## ¿Necesito presionar el botón reinvertir?

No. Alguien más lo presionará por Ud. para obtener la recompensa.

## ¿Cómo funciona?

El botón reinvertir toma todas las recompensas pendientes de un fondo, los convierte en un active de granja y los reinvierte nuevamente en el fondo para combinar depósitos para todos en la granja.

Hay una recompensa variable para incentivar a los usuarios a presionar ese botón. Quienquiera que sea el primero en presionar el botón, obtiene la recompensa y combina los depósitos de todos.

## ¿Cuándo debo presionarlo?

El botón reinvertir es opcional. No necesita presionarlo. Sin embargo, podría estar motivado a presionarlos para obtener la recompensa.

Si su objetivo es ganar neto en AVAX, entonces necesita considerar la relación entre token de recompensa / precio de AVAX, costo de transacción para reinvertir para ese fondo en particular, el costo de transacción por intercambiar el token de recompensa a AVAX, etc.

No necesita participar en el fondo para ser capaz de recibir la recompensa de reinversión. Cualquiera que presione el botón y complete la transacción recibirá la recompensa. Con eso en mente, puede ser competitivo, así que asegúrese de ser rápido.

## Ejemplo del Proceso de Reinversión

Así que por ejemplo, digamos que está en el fondo de abajo \(Pangolin ETH-AVAX / PEFI\). 

![](../.gitbook/assets/screen-shot-2021-05-14-at-9.06.18-pm.png)

Participando en este fondo, Ud. ha proporcionado liquidez en Pangolin en la forma de ETH y AVAX y Ud. ha depositado esos tokens LP en la granja de Yield Yak. Esos tokens LP están siendo depositadas en Penguin Finance y las recompensas para este fondo están dadas en PEFI.

Un re-inversionista presiona el botón cuando hay un balance pendiente de 100 PEFI.

* El re-inversionista cobra 3 PEFI \(dada una recompensa de 3%\)
* Tesorería cobra 5 PEFI \(dada una tasa de 5%\)
* Los PEFI restantes son reinvertidos

Los PEFI restantes son vendidos por ETH y AVAX, añadidos a los tokens LP de Pangolin y luego depositados nuevamente en el fondo.

## Más información

### Mecanismo de Protección

La función de reinversión contiene un mecanismo de protección para limitar que tan rápido ocurren dos reinversiones seguidas. Por diseño, la segunda transacción \(la cual casi no recibe recompensa\) debe fallar a un costo de gas bajo \(~0.03 AVAX\) en lugar de ser ejecutada con el uso de completo de gas.

Si no recibe casi ninguna recompensa porque alguien más fue ligeramente más rápido y su transacción fue exitosa, por favor sugiera a nuestro equipo un cambio a esta configuración.

### Falla de Transacción

Si encuentra una falla en la transacción después de presionar el botón reinvertir, esto es normal por una o dos razones:

1. De alguna manera Ud. logro presentar una transacción cuando la recompensa de token está por debajo del umbral mínimo. La tasa \(gas\) es relativamente baja de todos modos. \(~0.03 AVAX\).
2. De alguna manera el límite de gas por defecto para reinvertir no es suficiente para la transacción. Necesitará incrementar manualmente el límite de gas. Una falla debido a esto puede terminarle costando todo el límite de gas por defecto.

### Tasas

Las tasas son cobradas cada vez que una granja es combinada, desde los tokens de recompensa.

Las tasas son usualmente entre 5-10% de los tokens de recompensa. Las tasas son variables y cambian con las condiciones de la red para optimizar las recompensas. Hay tres categorías de tasas:

1. **Recompensa de Reinversión** - pagada al re-inversionista que presiona el botón
2. **Tasa de administración** - pagada a la red
3. **Tasa de desarrollador** - pagada al desarrollador que escribió la estrategia

Yield Yak no impone ninguna tasa de depósito o retiro \(aunque las granjas subyacentes podrían\).

  

