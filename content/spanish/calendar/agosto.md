---
title: "Agosto"
meta_title: "Tal dia como hoy en Bitcoin: Hitos y efemérides bitcoiners | Proyecto Bitcoin"
description: "Fechas más relevantes en el desarrollo de Bitcoin, mes a mes"
image: "images/banners/rojo.jpg"
categories: ["hitos", "calendario"]
tag: ["segwit", "vulnerabilidad", "minería", "PoW", "Hal Finney"]
date: 2024-07-29T00:21:53-04:00
draft: false
---

## 01-08-2017: Bitcoin Independence Day

El primero de agosto de 2017 termina, con triunfo para los usuarios, la **“Guerra de los Bloques”**. Desde ese momento se celebra, cada año, el **_Bitcoin Independence Day._**

{{< image src="images/efemerides/1-agosto.png" caption="" alt="Puño en alto en color negro, sobre un fondo naranja" height="" width="640" position="center" command="" option="q100" class="img-fluid" title="Bitcoin Independence Day"  webp="false" >}}

La también conocida como **“Guerra de los Bloques”** sentó un antes y un después en la vida de Bitcoin. **El problema de la escalabilidad, escaló (pun intended) y se convirtió en una batalla campal** en la que participaron nodos, empresas y mineros.

Agárrense que la historia es larga y tiene de todo: traiciones, errores bienintencionados, reuniones secretas y plot twist al final.

En 2009 Satoshi establece al tamaño del bloque un límite de 1 MB. ¿Por qué? Pues porque había que ponerlo en algún lado. Los bloques en ese tiempo pesaban pocos kilobytes, y algunos presumen que la idea era adelantarse a posibles ataques de DoS.

Jeff Garzik fué el primero en proponer un parche para solucionar el problema, el 3 de octubre de 2010. El parche era, en efecto, una hard fork que no se implementó. Se usó la rata de intercambios de PayPal de ese momento como el estándar a igualar.

{{< image src="images/efemerides/1-agosto-2.png" caption="" alt="Captura de pantalla bitcointalk" height="" width="1000" position="center" command="" option="q100" class="img-fluid" title="Propuesta de Jeff Garzik"  webp="false" >}}

La discusión continuó, sin traducirse en nada concreto. Se introdujeron los conceptos de Hard fork (donde el código nuevo es incompatible con el viejo y, en la realidad, se originan dos cadenas) y Soft fork (donde eso no ocurre).

Llegamos a mayo de 2015. Gavin Andressen and Mike Hearn toman el toro por los cuernos y proponen aumentar el tamaño del bloque a 20 MB (que por pedir no quede). Después se tranzaron en 8 MB.

Mike Hearn hace la propuesta de mejora BIP-101, con bloques de 8 MB y un mapa de rutas para lograrlo, pero se requería un Hard fork. Había nacido Bitcoin XT. La resistencia de la comunidad fue enorme y se lo acusó de un intento de “golpe de estado”.

Peter R Rizun presentó una charla en el encuentro Scaling Bitcoin (Fase I), que se llevó a cabo en Montreal en septiembre de 2015, en la que mostraba que se podía remover el límite del tamaño del bloque con seguridad.

En enero de 2016 él y Andrew Stone publicaron Bitcoin Unlimited, otro hardfork.

En ese mismo workshop, que estaba destinado a desarrolladores, Joseph Poon y Thaddeus Dryja proponen Lightning Network como solución alternativa a la escalabilidad. El white paper se publicaría en enero del año siguiente.

**SegWit se propuso como solución en diciembre de 2015,** por Peter Wuille, en el Scaling Bitcoin (Fase II) de Hong Kong. La propuesta traía un aumento significativo del tamaño de los bloques, solucionaba problemas de seguridad, tenía un mapa de rutas y solo implicaba un Soft fork.

{{< accordion "Fuentes" >}}

- <https://steemit.com/bitcoin/@tobixen/a-brief-history-of-the-bitcoin-block-size-war>
- <https://youtu.be/ON_R_lGTFu8>
- <https://www.criptonoticias.com/comunidad/aparecen-correos-satoshi-nakamoto-con-mike-hearn-escalabilidad-bitcoin/>
- <https://bitcointalk.org/index.php?topic=1391350.0>
- <https://github.com/jgarzik/bip100/blame/master/bip-0100.mediawiki>

{{< /accordion >}}

## 02-08-2016: Ataque a Bitfinex: segundo robo de bitcoin más grande a un exchage

El 2 de agosto de 2016 una vulnerabilidad en la estructura de cuentas de Bitfinex permitió a un atacante obtener acceso a las carteras de la plataforma. Un total de 119.756 BTC fueron robados.

**Bitfinex era, para el momento, una de las casas de cambio más grandes del mundo.** El valor de las criptomonedas era, al cambio, unos 60 millones de dólares. En la actualidad valdrían unos 4.751 millones de dólares.

{{< image src="images/efemerides/2-agosto-1.png" caption="" alt="Captura de pantalla Reuters" height="" width="640" position="center" command="" option="q100" class="img-fluid" title="Titular de Reuters sobre el robo"  webp="false" >}}

El robo de Bitfinex representó la mayor pérdida de bitcoin por un intercambio desde el evento ocurrido al, ahora infame, Mt Gox en Japón, donde se perdieron 744.408 BTC a principios de 2014.

La vulnerabilidad parece haber estado relacionada con la estructura multifirma implementada en alianza con BitGo para añadir seguridad a las cuentas.

BitGo reportó que sus servidores no habían sido vulnerados:

{{< image src="images/efemerides/2-agosto-2.png" caption="Fuente: <https://twitter.com/BitGo/status/760624908334346240>" alt="Captura Bitgo" height="" width="640" position="center" command="" option="q100" class="img-fluid" title="Anuncio de Bitgo en Twitter"  webp="false" >}}

Todos los servicios de intercambio fueron detenidos durante el proceso de investigación. El precio de Bitcoin cayó un 20% en un mercado que ya estaba a la baja antes del incidente.

{{< accordion "Fuentes" >}}

- <https://www.reddit.com/r/Bitcoin/comments/4vtuxo/bitfinex_security_breach_trading_will_be_halted/d61oelu/>
- <https://www.coindesk.com/bitfinex-bitcoin-hack-know-dont-know>
- <https://blog.bitgo.com/bitfinex-breach-update-2acf0e30719e>
- <https://mashable.com/article/bitfinex-hacked>
- <https://www.reuters.com/article/us-bitfinex-hacked-hongkong-idUSKCN10E0KP>

{{< /accordion >}}

## 15-08-2010: Explotan vulnerabilidad de Bitcoin

El 15 de agosto de 2010 una vulnerabilidad en el código de Bitcoin, que ya había sido detectada el 6 del mismo mes, fue explotada. Se generaron 184 mil millones de bitcoin en una transacción y se enviaron a dos direcciones en la red.

El problema fue detectado pocas horas después. Una vez corregido el problema se bifurcó la red principal, dejando por fuera los bloques que contenían las transacciones maliciosas

Hasta el día de hoy, este ha sido el único fallo grave del protocolo que haya sido encontrado y explotado

{{< accordion "Fuentes" >}}

- <https://nvd.nist.gov/vuln/detail/CVE-2010-5139>
- <https://es.wikipedia.org/wiki/Historia_de_bitcoin#2009>
- <https://iwillteachucrypto.medium.com/the-complete-history-of-bitcoin-how-satoshi-the-worlds-first-decentralized-came-to-be-d5c0ef1cb067>

{{< /accordion >}}

## 23-08-2017: Se activa segwit en la red principal

El 24 de agosto de 2017, a la altura del bloque 481824 se activa el soft- fork producto de la propuesta de mejora BIP14: Segregated Witness, o SegWit.

La Guerra de los Bloques, como se llamó a toda la polémica que terminó en la implementación de SegWit, fue un antes y después en la historia de Bitcoin. Uno de los efectos secundarios fue algo que hoy damos por sentado: La Bifurcación Suave Activada por Usuario (UASF)

{{< accordion "Fuentes" >}}

- <https://es.wikipedia.org/wiki/SegWit>
- <https://bravenewcoin.com/insights/bitcoin-scaling-solution-segwit-released>
- <https://bitcoincore.org/en/2016/10/27/release-0.13.1/>
- <https://cointelegraph.com/news/ready-steady-fork-bitcoin-core-to-release-segwit-in-november>
- <https://www.criptonoticias.com/mineria/segwit-esta-oficialmente-activado-red-bitcoin/>
- <https://mempool.space/es/block/0000000000000000001c8018d9cb3b742ef25114f27563e3fc4a1902167f9893>
- <https://twitter.com/CriptoNoticias/status/1686392166833123328>

{{< /accordion >}}

## 28-08-2014: Muere Hal Finney, primer minero de Bitcoin

El 28 de agosto de 2014 muere Hal Finney, creador, en 2004, del primer sistema de prueba de trabajo reutilizable y receptor de la primera transacción de Bitcoin.

{{< image src="images/efemerides/Hal_Finney_(computer_scientist).jpg" caption="" alt="Foto de Hal Finney, Científico de Datos " height="350" width="350" position="center" command="" option="q100" class="img-fluid" title="Hal Finney"  webp="false" >}}

Finney fue un contribuidor prolífico a la causa de la privacidad y los Cypherpunks, aportando a los sistemas de remails anónimos y a los sistemas de encriptación.

Le diagnosticaron ELA (esclerosis lateral amiotrófica) en el año 2009, siguió trabajando en código y anonimato hasta que se jubiló en el año 2011.

El 19 de marzo de 2013 publicó, en bitcointalk “Bitcoin y yo” un artículo donde relata su encuentro con la criptomoneda, lo mucho que le entusiasmaba y el trabajo que hizo para ayudar a Satoshi a mejorarla.

**Fue el primer minero, además de Satoshi,** y recibió de éste la primera transacción que se conoce: 1HLoD9E4SDFFPDiYfNYnkBLQ85Y51J3Zb1

{{< image src="images/efemerides/28-agosto-2.png" caption="Fuente: <https://twitter.com/halfin/status/1110302988>" alt="Captura del tuit de Hal Finney" height="" width="640" position="center" command="" option="q100" class="img-fluid" title="Corriendo Bitcoin"  webp="false" >}}

Falleció en Phoenix, Arizona, a consecuencia de las complcaiones de la ELA. Fue criopreservado en la Alcor Life Extension Foundation.

El famoso paciente 128.

{{< accordion "Fuentes" >}}

- <https://youtu.be/CNXW2sPuUrc?si=bhK8GRuMnKN-OoKZ>
- <https://alfre.info/blog/historiacrypto-1-cypherpunks-bitcoin/>
- <https://bitcointalk.org/index.php?topic=155054.0>
- <https://drive.google.com/file/d/1UJ_RjJgcmNng8lIGpo_VAfdu2fUZckx1/edit>
- <https://en.wikipedia.org/wiki/Hal_Finney_(computer_scientist)>
- <https://mempool.space/es/address/1HLoD9E4SDFFPDiYfNYnkBLQ85Y51J3Zb1>

{{< /accordion >}}

<hr>
