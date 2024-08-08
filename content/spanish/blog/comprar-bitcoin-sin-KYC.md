---
title: "Cómo Comprar Bitcoin Sin KYC: tutorial de Lnp2pbot"
meta_title: "Tutorial: como comprar y vender bitcoin usando LNP2Pbot | Proyecto Bitcoin"
description: "Aprende a usar un exchange p2p de bitcoin basado en Lightning, que no requiere entregar datos personales"
author: "Genny Díaz"
image: "images/tutorial-lnp2pbot-1280x720.jpg/"
categories: ['Mercado de bitcoin']
tags: ['Privacidad', 'p2p', 'exchange', 'tutorial']
date: 2024-08-08T13:31:31-04:00
draft: false
---

*En este tutorial aprenderemos a adquirir fracciones de bitcoin (satoshis) en la red Lightning Network, usando un exchange p2p sin registro de datos personales.*

<hr>

## Tutorial: uso básico LNp2pbot

El presente tutorial fue elaborado a principios de 2023 para el Seminario socrático de Mastering Bitcoin de [@libreriadesatoshi](https://twitter.com/libdesatoshi).

Puedes encontrar la documentación de referencia en la página web [LNp2pBot.com, sección "Aprende"](https://lnp2pbot.com/aprende/index.html)

Para correcciones, comentarios o sugerencias, escríbeme un DM en cuenta de X (Twitter): [@CriptoGenny](https://twitter.com/CriptoGenny) o [@ProyectBitcoin](https://twitter.com/ProyectBitcoin)

## Conceptos básicos

### ⚡ Lightning Network

Es un protocolo diseñado para realizar micropagos de bitcoin fuera de su blockchain. La red Lightning hace posibles transacciones de bitcoin instantáneas, pagando comisiones muy bajas.

### 💰 Satoshis

Un satoshi es una unidad más pequeña que un bitcoin. Una fracción equivalente a 0,00000001 BTC. Usualmente, lo encontrarás escrito con minúsculas: "satoshis", o abreviado: "sats".

### 💱 Exchange peer-to-peer (p2p)

Un exchange o mercado p2p (entre pares) es una plataforma donde los usuarios pueden comprar y vender bitcoin. Las transacciones se realizan directamente entre usuarios utilizando diferentes métodos de pago, incluyendo moneda local u otras criptomonedas.

### 🤖 LNp2pBot

Es una plataforma p2p que permite realizar intercambios de bitcoin por moneda local en la Lightning Network. Es un bot de Telegram que se puede usar sin registro de usuario ni verificación de identidad.

{{< image src="images/roboto-gif1.gif" caption="" alt="alter-text" height="" width="320" position="center" command="" option="q100" class="img-fluid" title="Roboto"  webp="false" >}}

## Requerimientos

Para interactuar con LNp2pBot se requiere una cuenta en la aplicación de mensajería Telegram con el *"username"* activado. También necesitas disponer de una wallet o monedero de bitcoin que soporte Lightning Network.

## Funcionamiento

- La herramienta LNp2pBot consta de dos partes:
    **1. El chat directo con el bot**. Es donde interactúas con la aplicación y le das instrucciones.
    **2. El canal de ofertas**. Aquí se publican las ofertas de compra y venta. El canal está conectado al bot.
- LNp2pbot es un sistema **"sin custodia"**, es decir, los satoshis no se mantienen depositados en la plataforma. Los pares usan monederos de Lightning bajo su control para realizar los intercambios.
- El bot opera usando una función nativa de la red Lightning llamada **"factura retenida"** **_(hodl invoice)_**. Esta función permite bloquear pagos en Lightning y liberarlos cuando se cumplan ciertas condiciones. Para saber más sobre esta función puedes visitar este enlace: [Hodl invoice](https://github.com/lightningnetwork/lnd/pull/2022).
- La plataforma cuenta con un **sistema de reputación** que ofrece estadísticas de los usuarios, como el total de operaciones exitosas y calificación recibida de sus pares en los intercambios.
- El bot cobra una **tarifa fija** de 0,6% por transacción, que incluye las comisiones de red.
- LNp2pbot también puede funcionar **dentro de un grupo o comunidad** de Telegram específica. Vinculándolo a tu grupo, te conviertes en administrador del bot en tu comunidad. El bot comparte la comisión por transacciones dentro de una comunidad con sus administradores. Para saber más sobre este tema, visita este enlace: [Comunidades en LNp2pbot](https://lnp2pbot.com/aprende/communities.html)

## Iniciar LNp2pBot

Abre la aplicación Telegram e introduce en la barra de búsqueda *"lnp2pbot"* para encontrar el chat directo con el bot. También puedes acceder directamente con este enlace: [@lnp2pbot](https://t.me/lnp2pbot).

Una vez que entres en el chat, presiona el botón *"Iniciar"*. Este procedimiento es necesario solo la primera vez que interactúes con el bot.

## Comprar satoshis

### Creando una orden de compra

Para comprar satoshis necesitarás crear una *"orden de compra"*. El bot cuenta con un asistente que te guiará en el proceso. Sigue estos pasos:

1. Haz clic en el botón *"Menú"* y selecciona la opción *"crear  ferta"*. También puedes escribir directamente el comando `/buy`
2. Especifica la moneda con la que pagarás los satoshis. El bot usa los códigos de divisa [ISO 4217](https://es.wikipedia.org/wiki/ISO_4217), escribe el correspondiente a tu moneda. Por ejemplo, "ARS" para pesos argentinos, "MXN" para pesos mexicanos, "USD" para dólares estadounidenses, etc.
3. Ingresa el monto de tu transacción.
4. Ahora escribe cuántos satoshis quieres recibir por tu dinero, o elige el botón *"Precio de mercado"* para que el bot haga el cálculo automáticamente. El bot aplicará la tasa de [Yadio.io.](https://yadio.io/)
5. En este punto, el bot te ofrece la opción de aplicar una prima o un descuento para hacer más atractiva tu oferta. Si quieres comprar por un precio superior al de mercado, selecciona un porcentaje de prima. Si quieres comprar más barato que el precio de mercado, selecciona un porcentaje de descuento. Si prefieres no usar esta opción, haz clic en el botón *"Sin prima ni descuento"*.
6. Finalmente, especifica el método de pago que usarás, por ejemplo: "trasferencia bancaria desde el banco XXXX"

#### 💡 Método abreviado

Puedes crear una orden de compra sin usar el asistente, enviando las instrucciones al bot en una sola línea, en forma de comandos:

- Primero detén el asistente usando: `/exit`
- Luego, escribe comando `/buy` seguido de los detalles de tu oferta. Cada dato debe ir separado por un espacio, sin caracteres especiales y respentando el orden:
`/buy <monto en sats> <monto en fiat> <código fiat> <método de pago> <prima/descuento>`
- El resultado se verá como en este ejemplo: `/buy 100000 50 usd "xxxx bank" -1`

Cumplidos estos pasos, el bot publicará tu oferta en el canal *"lnp2pbot Exchange"*. Espera que otro usuario la tome.

Si tu oferta no es tomada en un plazo de 23 horas, se cancelará automáticamente. También puedes cancelar la orden de compra en cualquier momento, escribiendo el comando `/cancel` más el ID de la orden. El bot te proporcionará este dato al publicar tu oferta.

Ejemplo: `/cancel 63e7f81086dc851f5fc4727d`

### Completando el intercambio

Una vez que un usuario toma tu orden de compra recibirás un mensaje de aviso en el chat. Entonces, procede a completar la transacción:

1. Abre tu wallet o cartera Lightning Network y crea una factura *(invoice)* con el monto en satoshis correspondiente a la orden de compra.
2. Copia y pega la factura en tu chat con el bot y presiona enviar. De inmediato, tu contraparte recibirá el aviso de que debe pagar esa factura. Una vez que lo haga, los satoshis permanecerán en estado de espera *(hold)* hasta que tu contraparte confirme que recibió el pago en fíat y los libere.
3. El bot pondrá en contacto a ambos usuarios. Solicita a tu contraparte la información de pago y procede a transferirle el correspondiente importe en fíat.
4. Una vez hecho el pago, envía al bot el comando `/fiatsent`. Tu contraparte recibirá una notificación para que verifique el pago y proceda a liberar los satoshis.
5. El bot te avisará cuando el vendedor libere los satoshis y te pedirá que califiques tu experiencia.

### Aceptando una oferta en el canal @lnp2pbot Exchange

Otra forma de adquirir satoshis en LNp2pBot es tomando una oferta publicada en el canal de compra/venta. En este caso solo tienes entrar al canal [@lnp2pbot Exchange](https://t.me/p2plightning) y buscar una oferta que se adapte a tus requerimientos. Una vez que la encuentres, pulsa el botón *"comprar satoshis"* que está al pie de la oferta y sigue los pasos de la sección: *"Completando el Intercambio"*

## ▶️ Videotutorial

En el siguiente enlace puedes ver el [Tutorial: Comprando bitcoin sin KYC con LNP2Pbot](https://youtu.be/dRzv7sLk8Wo)

## ⚡ Donaciones

Si te fue útil este material puedes agradecerme enviándo un aporte vía Lightning Address: *genny@getalby.com.*

<hr>
