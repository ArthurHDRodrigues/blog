---
layout: post
title: "LineageOS: Uma opção ao Android de fábrica para combater a obsolecência programada."
date: 2021-09-28 21:08:20 +0000
categories: jekyll update
---

## Sobre LineageOS

<a href="https://lineageos.org/">LineageOS</a> é uma ROM customizada (Custom ROM) livre e open-source de Android.
No presente momento, há suporte para celulares de 31 fabricantes e mais de 100 modelos.

Usar custom ROMs como esta permite dar uma vida nova a aparelhos mais antigos. Nunca instalei uma custom ROM, então para minha primeira experiência decidi tentar instalar em um Galaxy S6 Edge. Você pode consultar <a href="https://wiki.lineageos.org/devices/">a lista de aparelhos compartiveis</a>.
   
## Instalação
   
O processo de instalação foi surpreendentemente simples e rápido. Segui <a href="https://wiki.lineageos.org/devices/zeroltexx/install">esse tutorial da wiki para o Galaxy S6 Edge</a>.


Os dois únicos pontos necessários para comentar é que o link para o custom recovery dado pela wiki está fora do ar, procurando na rede achei o
<a href="https://twrp.me/samsung/samsunggalaxys6edge.html">link atual para o TWRP</a>; e    
como meu aparelho não é mais oficialmente suportado, precisei pegar uma <a href="https://www.los-legacy.de/17.1/zeroltexx">imagem não oficial</a>.

## Experiência de uso e de-google

Conseguir instalar outro OS no celular abre uma gama de opções, agora posso testar outras ROM, mais experimentais e que talvez não funcionem no meu dispositivo, como o kali netrunner generic, e se tudo der errado ainda posso voltar para o lineage.


Outra coisa que percebi é que sempre falamos de obsolecência programada e bla bla bla, mas conseguir instalar um Android 10 em um dispositivo que a fabricante <b>decidiu</b> abandonar no Android 7 me mostrou o quão real e forte é essa obsolecência e o quão importante é combate-la.

No final de 2021 meu celular quebrou e tive que usar o lineageOS como <i>Daily-Driver</i> enquanto guardava dinheiro para um celular novo. Pra isso, reformatei o celular e segui o mesmo tutorial para instalar a PlayStore em sideload, assim pude baixar apps proprietáros como os de bancos ou de redes sociais.


Toda a experiência de uso foi bem tranquila e agradável. Considerei seriamente em manter meu S6 edge como meu <i>Daily-Driver</i> até que quebrasse de vez, o único fator que me fez comprar outro celular é que a tela do S6 estava lascada e as vezes o touch parava de e voltava a funcionar do nada. 


Fazer de-google consiste em remover tudo da google de dispositivos, claro que instalar outra ROM em seu celular é o primeiro passo. O LineageOS <b>não</b> é 100% de-googled, <a href="https://www.youtube.com/watch?v=E1U5qoiR1fM">esse video</a> mostra como terminar o processo.

## Outras ROMs

Enquanto pesquisava por/sobre lineageOS, encontrei outras opções de ROMs que podem ser de interesse geral.
   
   
### postmarketOS
  
<a href="https://postmarketos.org/">postmarketOS</a> é na verdade uma distro de linux feita para rodar em celulares. A <a href="https://wiki.postmarketos.org/wiki/Devices">lista de aparelhos</a> é extensa, mas muitos dos dispositivos tem poucas funcionalidades implementadas, por exemplo, o port para o <a href="https://wiki.postmarketos.org/wiki/Samsung_Galaxy_S6_Edge_(samsung-zeroltexx)">S6 edge</a> não apresenta suporte para bluetooth, GPS Camera, bateria, etc. No entanto, parece ter <a href="https://gitlab.com/postmarketOS/pmaports/-/merge_requests/2105">um novo port</a> mais atual.
  
  
### Kali Netrunner
  
<a href="https://www.kali.org/get-kali/#kali-mobile">Kali Netrunner</a> é uma versão mobile do kali. Eles dão suporte oficial para pouquissimos aparelhos e obviamente Samsung S6 não é um deles. <a href="https://null-byte.wonderhowto.com/forum/kali-linux-samsung-galaxy-s6-0173997/">Nesse post </a>de forum aparentemente alguém consegui instalar uma versão genérica do OS. Também é possivel instalar <a href="https://www.kali.org/docs/nethunter/nethunter-rootless/">rootless usando termux</a>.
  
  
### Outras
- <a href="https://evolution-x.org/">evolution-x</a>
- <a href="https://grapheneos.org/">GrapheneOS</a>
