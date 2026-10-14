# 🧟 Sobreviventes — Guia Completo

RPG 2D de sobrevivência zumbi, visto de cima, em **um único arquivo HTML**. Funciona no PC e no celular, **offline** (sem internet), com áudio sintetizado e salvamento automático. Também tem **modo cooperativo online** para até 4 jogadores.

> Dica rápida: abra `index.html` (ou `sobreviventes.html`) no navegador, toque em **Novo jogo** e siga o tutorial. Se você morrer no modo solo, o save é apagado.

---

## Índice
1. [Como abrir e jogar](#1-como-abrir-e-jogar)
2. [Controles](#2-controles)
3. [Sobrevivência: fome, sede, energia, infecção](#3-sobrevivência)
4. [Combate e zumbis](#4-combate-e-zumbis)
5. [Explorar o mundo](#5-explorar-o-mundo)
6. [Inventário, peso e mochilas](#6-inventário-peso-e-mochilas)
7. [Construir abrigo](#7-construir-abrigo)
8. [Árvores, lenha e replantio](#8-árvores-lenha-e-replantio)
9. [Sobreviventes (NPCs)](#9-sobreviventes-npcs)
10. [Sobrevivência avançada](#10-sobrevivência-avançada)
11. [Fabricação](#11-fabricação)
12. [Catálogo de itens](#12-catálogo-de-itens)
13. [Progressão: nível, atributos e habilidades](#13-progressão)
14. [Missões](#14-missões)
15. [Dia, noite, clima e eventos](#15-dia-noite-clima-e-eventos)
16. [Modo celular](#16-modo-celular)
17. [Salvamento](#17-salvamento)
18. [Co-op online](#18-co-op-online)
19. [Publicar o jogo (GitHub Pages + Render)](#19-publicar-o-jogo)
20. [Dicas de sobrevivência](#20-dicas-de-sobrevivência)
21. [Problemas comuns](#21-problemas-comuns)

---

## 1. Como abrir e jogar

- **PC:** dê dois cliques no arquivo HTML. Funciona em Chrome, Edge, Firefox e Safari recentes.
- **Celular:** abra o arquivo (ou o link do site) no navegador. Use **Menu → Tela cheia** para ativar tela cheia e orientação horizontal.
  - No iPhone o navegador não oferece tela cheia: use *Compartilhar → Adicionar à Tela de Início* e abra pelo ícone.
- **Menu principal:** Continuar, Novo jogo, 🌐 Online, Opções e Como jogar.
- Você começa no **seu abrigo** (uma casa à esquerda do mapa) com um taco, comida, curativos e um **baú inicial** com martelo, tábuas, pregos e panos.

## 2. Controles

### 💻 PC
| Ação | Tecla |
| --- | --- |
| Mover | **WASD** ou setas |
| Mirar | **Mouse** |
| Atacar / atirar | **Clique** ou **Espaço** |
| Correr | **Shift** |
| Agachar | **C** |
| Interagir (abrir, revistar, dormir, conversar…) | **E** ou **F** |
| Recarregar | **R** |
| Inventário | **I** ou **Tab** |
| Mapa | **M** |
| Barricar porta/janela | **B** |
| Curar rápido | **H** |
| Trocar arma | **Q** ou roda do mouse |
| Missões / Fabricar | **J** / **K** |
| Pausa / sair do modo construção | **Esc** |

### 📱 Celular (horizontal)
- **Joystick** (canto inferior esquerdo): mover.
- **Botões à direita:** ⚔ Atacar, ✋ Usar, 👟 Correr (toque liga/desliga), 🔄 Recarregar, 🥷 Agachar, 🔨 Barricar, 🩹 Curar.
- **Arma** (embaixo, ao centro): toque para trocar.
- **Topo:** 🎒 inventário, 🗺 mapa, ⏸ pausa.

## 3. Sobrevivência

| Medidor | O que acontece |
| --- | --- |
| ❤ **Vida** | Zerou, você morre. |
| 🍖 **Fome** / 💧 **Sede** / 😴 **Energia** | Caem devagar com o tempo. Zerando, você perde vida. |
| 👟 **Fôlego** | Gasta ao correr e atacar. Sem fôlego o dano cai e a cadência piora. |
| 🩸 **Sangramento** | Tira vida aos poucos. Use curativo, antisséptico ou kit médico. |
| ☣ **Infecção** | Mordidas e arranhões podem infectar. Use **antibiótico** cedo (−35) ou o **soro experimental** (cura total). Antisséptico reduz 15. |

- **Dormir:** interaja com uma cama (🛏). Só dá para dormir com energia abaixo de 88% e sem zumbis perseguindo por perto. Dormindo o tempo passa mais rápido e a energia volta. Qualquer movimento ou ataque acorda você.
- **Fogueiras** 🔥 curam mais rápido quem fica perto e **queimam zumbis** que encostam. Alimente com lenha (E).
- **Itens úteis:** 🧃 comida e bebida restauram; ⚡ energético e ☕ café dão energia; 💉 adrenalina cura um pouco e dá muita energia.

## 4. Combate e zumbis

### Zumbis
| Tipo | Vida | Velocidade | Dano | Característica |
| --- | --- | --- | --- | --- |
| Zumbi comum | 50 | lento | 8 | Fraco, mas vem em grupo. |
| Corredor | 30 | muito rápido | 6 | Frágil e perigoso se você estiver sem fôlego. |
| Tanque | 170 | lento | 22 | Resistente. Recua pouco quando atingido. |
| Gritador | 75 | médio | 7 | Raro. **Grita e atrai a horda.** Carrega a **chave do bunker**. |

Quanto mais dias você sobrevive e quanto mais perto do centro do mapa, mais corredores e tanques aparecem.

### Como eles te percebem
- Eles **veem** você de perto e **ouvem barulho**: tiros, corrida, portas, combate, explosões.
- **Agachar** (C) reduz o ruído; a **chuva** abafa os passos; a habilidade **Furtividade** reduz ainda mais.
- Barulho atrai os zumbis até o local, mesmo que não vejam você. Use **iscas sonoras** 📢 para desviá-los.

### Armas corpo a corpo
| Arma | Dano | Alcance | Cadência (s) | Alvos | Barulho | Observação |
| --- | --- | --- | --- | --- | --- | --- |
| 🔪 Faca | 15 | 36 | 0.38 | 1 | 70 | Rápida e silenciosa. |
| 🏏 Taco de beisebol | 21 | 46 | 0.6 | 2 | 110 | Equilibrado. Acerta até 2 alvos. |
| 🪓 Machado | 36 | 44 | 0.85 | 2 | 130 | Forte. Também corta árvores. |
| 🔨 Martelo | 23 | 38 | 0.55 | 1 | 100 | Necessário para barricar e fabricar. |
| 🔧 Pé de cabra | 26 | 42 | 0.65 | 1 | 110 | Arma e ferramenta: força portas trancadas. |
| 🔱 Lança improvisada | 20 | 68 | 0.7 | 1 | 80 | Longo alcance. |
| 🏏 Taco com pregos | 31 | 46 | 0.65 | 2 | 120 | Taco reforçado com pregos. |
| 🍳 Frigideira | 17 | 36 | 0.5 | 1 | 90 | Barulhenta, mas melhor que os punhos. |
| 🗡️ Facão | 29 | 50 | 0.55 | 2 | 90 | Rápido e afiado. Acerta até 2 alvos. |
| 🔨 Marreta | 50 | 46 | 1.15 | 2 | 140 | Pesada e brutal. Empurra tudo para trás. |
| ⚔️ Katana | 37 | 54 | 0.42 | 2 | 60 | Rara. Rápida, longa e silenciosa. |
| 🪈 Cano de ferro | 27 | 46 | 0.6 | 2 | 120 | Pesado e barato. Bate forte. |
| 🪓 Machado de incêndio | 46 | 50 | 0.95 | 2 | 140 | Brutal. Também corta árvores. |
| ⛏️ Picareta | 34 | 48 | 0.9 | 1 | 130 | Perfura crânios e também corta árvores. |
| 🪏 Pá | 25 | 50 | 0.75 | 2 | 110 | Pesada e longa. Acerta até 2 alvos. |
| 🏑 Clava de madeira | 24 | 44 | 0.62 | 2 | 105 | Tronco lapidado. Empurra bem. |
| 🥊 Soco inglês | 15 | 28 | 0.28 | 1 | 55 | Muito rápido e discreto. |
| 🔧 Chave inglesa | 24 | 40 | 0.6 | 1 | 110 | Arma e ferramenta de mecânico. Ajuda a consertar veículos. |
| 🔪 Cutelo | 31 | 38 | 0.5 | 1 | 85 | Pesado e cortante. |
| 🏑 Cassetete | 19 | 42 | 0.36 | 1 | 70 | Rápido e discreto. |
| 🪚 Motosserra | 15 | 42 | 0.12 | 3 | 430 | Raríssima. Dilacera hordas, mas é MUITO barulhenta. |
| 🔧 Chave de fenda | 14 | 30 | 0.3 | 1 | 50 | Pequena, rápida e silenciosa. |
| 📏 Atiçador de ferro | 22 | 52 | 0.5 | 1 | 80 | Haste de ferro de lareira. |
| 🏌️ Taco de golfe | 25 | 60 | 0.55 | 1 | 85 | Longo alcance e bom empurrão. |
| 🏒 Taco de hóquei | 23 | 56 | 0.45 | 1 | 80 | Leve e rápido. |
| 🥋 Tonfa policial | 21 | 40 | 0.32 | 1 | 60 | Rápida, controla a distância. |
| 🗡️ Sabre | 33 | 56 | 0.4 | 2 | 55 | Rara. Corte limpo e silencioso. |
| 🔨 Martelo de guerra | 54 | 44 | 0.95 | 2 | 130 | Lento, mas esmaga qualquer coisa. |
| 🌾 Foice | 36 | 62 | 0.7 | 3 | 75 | Corta vários zumbis num arco largo. |
| 🔱 Maça de pregos | 40 | 44 | 0.75 | 2 | 110 | Bola de aço com pontas. |
| 🔱 Forcado | 29 | 62 | 0.62 | 2 | 85 | Dois dentes e bom alcance. |
| 📏 Vergalhão | 26 | 50 | 0.55 | 1 | 95 | Barra de aço dobrada. |
| 🪓 Machadinha | 30 | 40 | 0.42 | 1 | 70 | Leve e afiada. Ótima para golpes furtivos. |
| 🔪 Faca de caco | 15 | 28 | 0.3 | 1 | 35 | Improvisada. Silenciosa; mata furtivo. |
| 🦯 Bengala de ferro | 21 | 52 | 0.45 | 1 | 75 | Surpreendentemente útil. |
| 🥋 Nunchaku | 24 | 44 | 0.3 | 2 | 70 | Rápido e imprevisível. |
| 🗡️ Baioneta | 26 | 38 | 0.34 | 1 | 45 | Lâmina militar. Furtiva. |

- Dano sobe com a habilidade **Corpo a corpo** (+8% por nível) e o atributo **Força**.
- **Machado** corta árvores; **pé de cabra** arromba portas trancadas; **martelo** barrica e desmonta construções.

### Armas de fogo
| Arma | Dano | Pente | Munição | Alcance | Barulho | Observação |
| --- | --- | --- | --- | --- | --- | --- |
| 🔫 Pistola 9mm | 30 | 12 | Munição 9mm | 380 | 720 | Precisa de munição 9mm. |
| 🔫 Espingarda | 15×7 | 6 | Cartucho calibre 12 | 230 | 850 | Devastadora de perto. Muito barulhenta. |
| 🎯 Rifle | 58 | 8 | Munição 7.62 | 560 | 950 | Longo alcance, atravessa alvos. |
| 🔫 Revólver .357 | 48 | 6 | Munição .357 | 420 | 880 | Potente. Precisa de munição .357. |
| 🔫 Submetralhadora | 19 | 30 | Munição 9mm | 300 | 800 | Rajadas rápidas com munição 9mm. Gasta muito. |
| 🏹 Besta | 55 | 1 | Virote | 420 | 40 | Quase silenciosa. Usa virotes. |
| 🔫 Fuzil de assalto | 34 | 30 | Munição 7.62 | 480 | 960 | Raríssimo. Rajada rápida com munição 7.62. |
| 🔫 Espingarda de cano duplo | 17×8 | 2 | Cartucho calibre 12 | 210 | 900 | Dois tiros devastadores seguidos. |
| 🏹 Arco | 42 | 1 | Flecha | 400 | 30 | Silencioso. Usa flechas. |
| 🎯 Rifle de precisão | 95 | 5 | Munição 7.62 | 760 | 980 | Raríssimo. Dano enorme a longa distância. |
| 🔫 Magnum .357 automática | 72 | 7 | Munição .357 | 460 | 930 | Raríssima. Dano enorme, estrondo enorme. |
| 🔫 Pistola compacta | 27 | 17 | Munição 9mm | 360 | 690 | Carregador grande. Munição 9mm. |
| 🔫 Mini submetralhadora | 16 | 32 | Munição 9mm | 260 | 780 | Cadência altíssima e pouca precisão. |
| 🔫 Rifle de alavanca | 52 | 8 | Munição .357 | 500 | 900 | Clássico e preciso. Usa munição .357. |
| 🔫 Espingarda de cano serrado | 14×9 | 2 | Cartucho calibre 12 | 150 | 930 | Curto alcance, dano brutal e muito barulho. |
| 🔫 Carabina | 40 | 15 | Munição 7.62 | 520 | 940 | Meio-termo entre o fuzil e o rifle. Munição 7.62. |
| 🏹 Arco composto | 58 | 1 | Flecha | 480 | 30 | Silencioso, potente e preciso. Usa flechas. |
| 🔫 Submetralhadora MP5 | 22 | 30 | Munição 9mm | 340 | 780 | Mais precisa que a SMG comum. |
| 🔫 Pistola pesada | 36 | 8 | Munição 9mm | 370 | 760 | Pouca munição, mas bate forte. 9mm. |
| 🔫 Rifle de caça | 70 | 5 | Munição 7.62 | 620 | 900 | Ferrolho: lento e muito preciso. 7.62. |
| 🔧 Pistola de pregos | 20 | 24 | Prego | 200 | 120 | Usa pregos como munição. Bem silenciosa. |

- Precisam de **munição** e **recarga** (R). A recarga automática começa quando o pente esvazia e você tem balas.
- A **besta** é quase silenciosa — ótima para furtividade. Fabrique virotes com lenha + sucata.
- Habilidade **Precisão** reduz a dispersão; agachar também. Correr e estar sem energia pioram a mira.
- 🛢 **Barris vermelhos explodem!** Atire neles de longe para atingir zumbis. Cuidado perto de **postos de gasolina**.

### Arremessáveis
- 💣 **Granada caseira:** explode ~2 s depois de lançada. O alcance da explosão também te machuca.
- 🔥 **Coquetel molotov:** cria um incêndio ~1 s depois de lançado, que queima zumbis.
- 📢 **Isca sonora:** faz barulho por alguns segundos no local onde cai.
- Todos são lançados na direção em que você olha, até uns 7 quadrados, parando antes de paredes.

### Fugir e se defender
- Feche portas e **barricade** (🔨/B) com tábuas e pregos: cada uso reforça mais (até 3 camadas).
- Zumbis quebram **janelas** para entrar; barricar a janela impede isso.
- Casas com porta fechada e fogueiras ajudam a ganhar distância; correr gasta fôlego, então alterne com andar.

## 5. Explorar o mundo

O mapa é uma cidade enorme (**992×992 quadrados**, 40×40 quarteirões — cerca de 2,7× a área da versão anterior e mais de 60× a primeira; saves antigos continuam com o tamanho em que foram criados: 128, 176, 248, 416 ou 608) com ruas, quarteirões, florestas, parques e lagos. Os locais mais importantes são marcados no mapa quando você os descobre:

| Local | O que tem |
| --- | --- |
| 🏠 **Casas** | Geladeiras, armários, camas, às vezes caixotes. Algumas portas são trancadas. |
| 🏥 **Hospital** | Muitos remédios, kits médicos, soro. Também muitos zumbis (inclusive tanques). |
| 🚔 **Delegacia** | Porta trancada (pé de cabra). Armas e munição. |
| 🛒 **Supermercado e lojas** | Comida e bebida em prateleiras. |
| 🔨 **Loja de ferragens** | Tábuas, pregos, ferramentas, machados, combustível. |
| ⛽ **Posto de gasolina** | Lanches, energéticos, combustível, mapas — e barris explosivos. |
| 🚜 **Celeiro** | Comida, cordas, ferramentas, mudas. |
| 🌲 **Cabanas na floresta** | Pouco saque, mas seguras. |
| 🏫 **Escola** | Mesas de professor e armários: lanches, pilhas, fita, mochilas, mapas. Muitos zumbis. |
| 🏭 **Armazém** | Porta trancada (pé de cabra). Estantes cheias de sucata, metal, fio, engrenagens, baterias, armadilhas e até bancadas. Barris explosivos do lado de fora. |
| 🧪 **Laboratório** | Porta interna trancada. Químicos, álcool, antibióticos, soro, vitaminas, baterias — e um tanque à espreita. |
| ⛪ **Igreja** | Pouco perigo: água, pão, mel, ervas, vitaminas e antibiótico ocasional. |
| 🔧 **Oficina mecânica** | Caixas de ferramentas e estantes: galões, kits de reparo, chaves inglesas, peças. Carros estacionados na frente. |
| 🏬 **Shopping** | Prédio enorme com muitas prateleiras (roupas, mochilas, eletrônicos, comida) e zumbis. Estacionamento com carros. |
| 🚗 **Ferro-velho** | Pátio cercado cheio de carcaças (porta-malas revistáveis), barris explosivos e alguns carros que funcionam. |
| 🏞️ **Lagos** | Água para **pescar** e coletar água suja; cabana na margem. |
| 🏚 **Bunker militar** | Trancado com a **chave do Gritador**. O melhor saque do jogo. |

- **Revistar** (E): armários, geladeiras, caixotes, mochilas abandonadas, porta-malas de carros. Leva alguns segundos e faz um pouco de barulho. Depois de revistado, o recipiente pode ser reaberto livremente.
- 🚁 **Helicópteros** podem largar caixas de suprimentos (aparecem no mapa como pontos dourados).
- 🔍 **Zoom no mapa:** roda do mouse, pinça (celular) ou os botões **Zoom ＋/－**; arraste para mover, **⌖ Eu** centraliza em você e **Mapa todo** volta à visão geral. Até 24×. Veículos já vistos aparecem como quadradinhos coloridos.
- 🗺️ O **mapa** só mostra o que você já explorou. O item **Mapa da região** revela uma grande área de uma vez.

## 6. Inventário, peso e mochilas

- Você tem **12 espaços** e **15 kg** de base.
- **Força** aumenta a carga (+2 kg por ponto).
- **Mochilas** (equipe pelo inventário) aumentam espaços e peso:

| Mochila | Espaços | Peso extra |
| --- | --- | --- |
| 🎒 Escolar | +6 | +8 kg |
| 🎒 De trilha | +9 | +13 kg |
| 🎒 Militar | +12 | +18 kg |
| 🎒 Tática | +18 | +28 kg |

- Itens empilham até o limite de cada um. Se não couber, o que sobrar cai no chão.
- 🔦 A **lanterna** funciona só por estar na mochila: aumenta muito a visão à noite.
- **Baús** guardam itens no abrigo, sem peso.

## 7. Construir abrigo

Fabrique os itens de construção (veja a [tabela](#11-fabricação)): 🧱 **parede de madeira**, 🚪 **portão de madeira**, 🛏️ **cama de abrigo**, além de 🧳 **baú** e 🔥 **fogueira**.

### Modo de construção (grade)
1. No inventário, selecione o item e toque em **Posicionar (grade)**.
2. Aparece uma **grade** ao redor de você (alcance de ~6 quadrados). **Verde** = pode colocar, **vermelho** = não pode. Uma prévia mostra o item no quadrado escolhido.
3. **PC:** clique no quadrado. **Celular:** toque no quadrado (a prévia vai para lá) e toque de novo, ou use o botão **✔ Colocar**.
4. Continue colocando enquanto tiver o item. Saia com **Esc**, clique direito ou o botão **✖ Sair**.
- Você pode **andar** enquanto está no modo de construção.
- Não dá para construir em cima de pessoas, zumbis, água, ruas ou objetos.
- **Portões** são desenhados na direção das paredes vizinhas: construa as paredes primeiro.

### Desmontar
Com o **🔨 martelo equipado**, o botão **Usar** (E) aparece como **Desmontar parede/portão/cama** nas construções feitas por você, e devolve o item. Também **arranca mudas**. Construções do mapa não podem ser desmontadas.

### Outros itens de construção
O mesmo modo de grade vale para 🌾 **sementes**, 🪤 **armadilhas de urso** e 🛠️ **bancada de trabalho** (veja a seção 10). Com o martelo você desmonta bancadas e armadilhas suas.

### Barricar o abrigo
Portas e janelas (inclusive as suas) podem ser barricadas com 🔨 / **B** (tábuas + pregos). Os zumbis não atravessam paredes construídas; eles precisam de portas abertas ou janelas quebradas.

## 8. Árvores, lenha e replantio

- Equipe um **🪓 machado** e use **Cortar árvore** (E). Cada árvore dá **2–3 lenha** e, com boa chance, **uma 🌱 muda**. A árvore vira um **toco**.
- A lenha vira **tábuas** (martelo) e **fogueiras**.
- **Replantar:** posicione a 🌱 muda em **grama, terra ou toco**. Em **2 a 3 minutos** ela vira uma árvore de novo.
- Cortar árvores faz barulho: cuidado com zumbis por perto.

## 9. Sobreviventes (NPCs)

> **Somente no modo offline.** No co-op online não há NPCs.

1. **Construa um abrigo:** coloque ao menos **uma cama sua** e algumas paredes/portões (o jogo considera cama + paredes). *Camas de casas do mapa nunca contam, só as que você construiu.*
2. Depois de alguns instantes, **um sobrevivente aparece ao longe** e vem até o abrigo, procurando um lugar. Se não houver cama livre, ele **espera por perto** (com o balão 🛏️?).
3. **Ofereça abrigo construindo uma cama extra.** Ele aceita na hora e se muda para ela.
4. A cama passa a ser dele ("Cama de *Nome*") e você não dorme nela. Ele fica perto, descansa à noite e **ajuda a defender** o abrigo atacando zumbis próximos (e pode morrer).
5. **Converse** com ele (E). Quando aparece o 🎁, ele te dá **comida e, às vezes, armas**. Um presente novo a cada dia; quanto mais convive, melhores os presentes.
- Se você **desmonta a cama** dele, ele volta a procurar abrigo.
- Se ele não achar o caminho até a cama, o jogo avisa: abra uma porta ou remova uma barricada.
- Até **6 sobreviventes** por jogo, um por cama.

| Profissão | Costuma dar |
| --- | --- |
| Cozinheira | Comida e bebida |
| Caçador | Carne seca, facas, facão, besta e virotes |
| Médica | Curativos, analgésicos, antibióticos, kits médicos |
| Ex-soldado | Munição e armas de fogo, granadas |
| Mecânico | Sucata, pregos, tábuas, metal, ferramentas |
| Fazendeira | Frutas, pão, água, mudas, lenha |

## 10. Sobrevivência avançada

### 🎣 Pesca e água
- **Vara de pesca** (🪵 2 lenha + 🪢 corda + 🪝 anzol): com ela na mochila, chegue perto da água e use **Pescar**. Leva alguns segundos; pode vir peixe, lixo útil ou nada.
- **Água suja**: com uma 🍾 garrafa vazia, use **Coletar água suja** perto de um lago. Beber suja pode fazer mal; **ferva** numa fogueira (receita) para virar água potável.
- Comida **crua** (peixe, carne) pode te deixar enjoado. Cozinhe antes.

### 🔥 Cozinhar
Receitas marcadas com 🔥 só funcionam **perto de uma fogueira acesa**: peixe assado, carne assada, ferver água, carne seca e **ensopado** (a refeição mais nutritiva).

### 🌾 Fazenda
Posicione **sementes** (modo de construção) em **grama ou terra**. A planta cresce em **3 estágios (~4 minutos)**, mais rápido na chuva. Quando amadurecer, use **Colher**: rende milho, tomate ou batata e, na maioria das vezes, sementes de volta. Milho também vira sementes. Fazendas e celeiros têm sementes e comida.

### 🏹 Caça (modo offline)
Coelhos 🐇, cervos 🦌 e **javalis** 🐗 vagam pelos campos. Coelhos e cervos fogem; o **javali ataca** se for ferido. Abatidos, dão 🥩 carne, 🟫 couro e 🦴 ossos. Armas silenciosas (besta, faca) não atraem zumbis. Em co-op não há animais.

### 🪤 Armadilhas de urso
Posicione no chão (grade). Zumbi que pisa leva **muito dano e fica preso ~6 s**; ela dispara uma vez. Use **Armar/Desarmar** (Usar) para rearmar. **Você também pode pisar nelas** (dano, sangramento e preso 2,5 s) — **agache** (C) para passar por cima com segurança. Em co-op, só o anfitrião aciona armadilhas ao pisar.

### 🛠️ Bancada de trabalho
Receitas marcadas com 🛠️ exigem estar **a até 3 quadrados de uma bancada**: coletes, chapas de metal, marreta, munição caseira (9mm e cartucho 12), antibiótico e baterias.

### 🛡️ Armaduras
Uma armadura por vez (botão **Vestir armadura**; **tirar** aparece no topo do inventário). Reduz todo dano recebido:

| Armadura | Redução | Observação |
| --- | --- | --- |
| 🧥 Jaqueta de couro | −14% | Fabricável (couro + pano + corda) |
| 🦺 Colete improvisado | −26% | Fabricável na bancada |
| 🛡️ Colete balístico | −40% | Melhora o colete na bancada ou acha-se em polícia/militar |
| 🥋 Traje antimotim | −52% | Raríssimo; você anda um pouco mais devagar |

Há também um **slot de capacete** separado (⛑️ ciclista −6%, 🪖 militar −13%) que **soma** com a armadura. Os dois aparecem com o botão **tirar** no topo do inventário.

### 💣 Arremessáveis
Molotov, granada, 💥 **bomba caseira** (explosão dupla), 🧨 **bombinhas** (estouros que atraem zumbis para longe de você) e 🌫️ **bomba de fumaça** (desorienta zumbis num raio de 7 quadrados por ~5 s). Arremesse pelo inventário; todos fazem barulho ao explodir, menos a fumaça.

### 📻 Rádio de emergência
Com uma 🔋 bateria e **ao ar livre** (fora de prédios), use o rádio: em **~45 s** um helicóptero larga uma caixa de suprimentos perto de você (aparece no mapa). O chamado faz **barulho** e pode atrair zumbis — prepare-se.

### 🪟 Quebrar vidro
- **Golpeie uma janela** com qualquer arma ou os punhos, ou use **Quebrar janela** (E) para quebrar de uma vez.
- Com **pano** na mão a quebra é **silenciosa**; com arma o barulho é alto; **de mão limpa sem pano** você se corta.
- Atravessar uma janela quebrada **em pé** pode cortar você (sangramento). **Agache** (C) para passar sem se ferir.
- Janelas barricadas não quebram até você remover as tábuas.

### 🚗 Dirigir veículos
- **Três tipos de veículo** (aparecem espalhados pelo mapa):
  - 🚗 **Carro:** equilibrado, 4 lugares.
  - 🏍️ **Moto:** a mais rápida e ágil (até ~390), gasta pouco combustível, mas é **frágil** (bate e quebra fácil) e o piloto se machuca mais nas batidas. Só 2 lugares (piloto + garupa).
  - 🚚 **Caminhão:** lento e pesado (~235), **muito resistente** (leva só ~55% do dano), atropela com mais força e gasta mais combustível. 4 lugares (2 na cabine, 2 na caçamba).
- **Serviços no veículo:** com o **agachado (C)** perto do veículo, a interação passa a oferecer **Abastecer**, **Consertar** e **Sifonar combustível** (em vez de Entrar). Sifonar precisa de uma **mangueira** e rende 1 ⛽ combustível por vez (−20% do tanque).
- **Carros** ficam estacionados nas ruas (cerca de metade de um por quarteirão), mais alguns no ferro-velho, oficina e shopping. Chegue perto e use **Entrar no veículo** (E). O mapa mostra a % de combustível ⛽ e de vida 🔧 no texto da interação.
- **Controles:** `W/S` ou ↑/↓ acelera e freia (ré), `A/D` ou ←/→ vira, `Espaço` = freio de mão, `H` = buzina, `E` = sair. **Celular:** joystick para cima/baixo acelera/freia, esquerda/direita vira, botão de ataque = freio.
- **Combustível:** gasta mais acelerando forte. Reabasteça com 🛢️ **galão de gasolina** (+60) ou ⛽ **combustível** (+20): use perto do carro (ou o botão **Abastecer** na interação). Sem combustível o carro para.
- **Dano:** batidas em paredes, árvores e outros carros machucam o carro e, em alta velocidade, **você**. Com pouca vida o carro fumega; a 0 ele **explode** e você leva dano de explosão. Conserte com 🛠️ **kit de reparo** (+50) ou **3 sucatas** (+18, +10 com chave inglesa).
- **Atropelar zumbis:** em velocidade (> ~55 px/s) o carro causa dano proporcional e arremessa zumbis; tanques desgastam o carro mais.
- **Barulho:** o motor atrai zumbis (mais rápido = mais barulho) e a buzina atrai muitos. Dentro do carro você recebe só ~35% do dano de zumbis (o carro absorve o resto).
- À noite os faróis iluminam bem mais. Você **não pode atacar nem construir** dirigindo.
- **Co-op:** todos veem os carros. Cada carro tem **4 lugares: 1 motorista e 3 passageiros**. Quem chega primeiro vira motorista; os outros usam **Entrar como passageiro**. Se o motorista sai, um passageiro assume o volante. Convidados também podem dirigir (o anfitrião calcula a física). Passageiros veem as barras de combustível/vida e saem com E. Só dá para entrar com o carro devagar. Combustível e conserto funcionam para todos.

### 🧱 Quebrar paredes
- **Derrube qualquer parede** (de casas, lojas, prédios e as que você construiu) para abrir atalhos ou fugir. Só o **bunker militar** e a borda do mapa são indestrutíveis.
- **Como:** equipe uma ferramenta pesada e use **Derrubar parede** (E) perto dela, ou simplesmente **golpeie** a parede. Cada golpe mostra rachaduras e a % de dano. Quebrada, a parede some, vira piso e solta 🔩 sucata (e às vezes tábuas/metal; as suas soltam tábuas e pregos).
- **Eficácia por arma:** 🔨 marreta e ⛏️ picareta (3–4 golpes), 🪓 machados, 🪚 motosserra (rapidíssima, barulhenta); 🔧 pé de cabra e cano funcionam devagar; tacos, facas e punhos quase não adiantam. Armas de fogo não afetam paredes.
- **Explosões** (granada, bomba caseira, barril vermelho) também danificam paredes num raio de ~3 quadrados.
- **Barulho alto** a cada golpe: os zumbis ouvem. Paredes (as suas também) valem pontos de abrigo: se você demolir sua parede, o abrigo perde proteção.
- Em co-op, o anfitrião valida os golpes dos outros jogadores.

### 🗝️ Arrombar portas com gazua
- Portas trancadas das casas pedem pé de cabra (barulhento, 3 s). Com uma **gazua** (🗝️) na mochila, a interação vira **Arrombar tranca**: leva ~2–4 s, é **quase silenciosa** e a chance de sucesso sobe com a habilidade **Garimpo** (de 56% até 95%). Falhar pode **quebrar a gazua (30%)**.
- Se você tiver pé de cabra **e** gazua, a gazua é usada quando você está **agachado**; em pé usa o pé de cabra.
- Fabrique: 📎 **grampos** (de arame) → **gazua** (3 grampos + metal).

### 🗡️ Golpe furtivo
- **Agachado**, chegue **por trás** de um zumbi que ainda **não te percebeu** e ataque com lâmina (faca, faca de caco, machete, katana, cutelo, chave de fenda, sabre, machadinha, baioneta; machado também funciona, mais fraco). O golpe causa dano multiplicado e **mata na hora** (menos Tanques, que levam um dano enorme). Treina **Furtividade**.

### 🧤 Equipamento de proteção
- 🧤 **Luvas** (na mochila): quebrar vidro ou pisar em cacos **não corta sua mão**.
- 🥾 **Botas reforçadas** (na mochila): menos de um terço da chance de se cortar em cacos e **metade do dano** de armadilha de urso.
- 🥼 **Traje de proteção**: reduz 28% do dano e deixa a **infecção 70% mais difícil**.
- 😷 **Máscara de gás**, 🧢 gorro, 🪖 capacete com viseira e outros novos capacetes/armaduras entram nos mesmos espaços de equipamento.
- 🔭 **Binóculos** e 🪢 **mangueira** são itens de uso passivo (mantenha na mochila).

### 💨 Gases e bombas de som
- 💨 **Gás lacrimogêneo:** nuvem por ~10 s num raio médio que **atordoa e fere** os zumbis.
- 🤢 **Bomba de fedor:** gera barulho enorme por vários segundos e **atrai** zumbis para longe de você — jogue longe e saia pelo outro lado.

### 🔧 Pistola de pregos
- Usa **pregos** como munição (24 por carregador), é **quase silenciosa** e tem bom dano para o barulho. Fabricada na bancada.

### 🏕️ Habilidade Sobrevivência
Sobe ao pescar, colher, caçar e cozinhar: pesca mais rápida, mais peixes, colheitas e caças maiores e menor chance de passar mal com comida crua.

## 11. Fabricação

Abra o menu **🔨 Fabricar** (K). As receitas aparecem em vermelho quando falta algo. Algumas exigem **martelo no inventário** e um **nível de Fabricação** mínimo.

| Resultado | Ingredientes | Nível de fabricação | Exige |
| --- | --- | --- | --- |
| 🩹 Curativo | 2× 🧵 Pano | 1 | — |
| 📏 Tábua ×2 | 1× 🌲 Lenha | 1 | 🔨 martelo |
| 📌 Prego ×5 | 2× 🔩 Sucata | 1 | — |
| 🏕️ Fogueira | 3× 🌲 Lenha | 1 | — |
| 📢 Isca sonora ×2 | 2× 🔩 Sucata, 1× 🧵 Pano | 2 | — |
| 🔱 Lança improvisada | 2× 🌲 Lenha, 1× 🔩 Sucata, 1× 🧵 Pano | 2 | — |
| 🧳 Baú | 6× 📏 Tábua, 6× 📌 Prego | 2 | 🔨 martelo |
| 🏏 Taco com pregos | 1× 🏏 Taco de beisebol, 5× 📌 Prego | 3 | 🔨 martelo |
| 🎒 Mochila escolar | 8× 🧵 Pano, 2× 🔩 Sucata | 4 | — |
| 🧰 Kit médico | 3× 🩹 Curativo, 1× 💊 Antibiótico, 2× 🧵 Pano | 5 | — |
| 🪢 Corda | 3× 🧵 Pano | 1 | — |
| 🔻 Virote ×4 | 1× 🌲 Lenha, 1× 🔩 Sucata | 2 | — |
| 🔥 Coquetel molotov | 1× 🍾 Garrafa vazia, 1× ⛽ Combustível, 1× 🧵 Pano | 2 | — |
| 🗡️ Facão | 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva, 1× 🌲 Lenha | 3 | 🔨 martelo |
| 💣 Granada caseira | 2× ⚫ Pólvora, 2× 🔩 Sucata, 1× 🧷 Fita adesiva | 4 | — |
| 🏹 Besta | 3× 🌲 Lenha, 2× 🪢 Corda, 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 4 | 🔨 martelo |
| 🎒 Mochila de trilha | 6× 🧵 Pano, 2× 🪢 Corda, 1× 🧷 Fita adesiva | 3 | — |
| 🎒 Mochila tática | 1× 🎒 Mochila de trilha, 2× 🪢 Corda, 1× 🔲 Chapa de metal, 2× 🧷 Fita adesiva | 6 | — |
| 🧴 Antisséptico | 1× 🧪 Álcool, 1× 🧵 Pano | 2 | — |
| 🧱 Parede de madeira ×2 | 2× 📏 Tábua, 3× 📌 Prego | 1 | 🔨 martelo |
| 🚪 Portão de madeira | 4× 📏 Tábua, 6× 📌 Prego | 1 | 🔨 martelo |
| 🛏️ Cama de abrigo | 4× 📏 Tábua, 6× 🧵 Pano, 4× 📌 Prego | 2 | 🔨 martelo |
| 🍣 Peixe assado | 1× 🐟 Peixe cru | 1 |  🔥 fogueira |
| 🍖 Carne assada | 1× 🥩 Carne crua | 1 |  🔥 fogueira |
| 💧 Garrafa d’água | 1× 🫗 Água suja | 1 |  🔥 fogueira |
| 🍲 Ensopado | 1× 🥩 Carne crua, 1× 🥔 Batata, 1× 🫗 Água suja | 2 |  🔥 fogueira |
| 🥓 Carne seca ×2 | 2× 🥩 Carne crua | 2 |  🔥 fogueira |
| 🪝 Anzol ×2 | 1× 🔩 Sucata | 1 | — |
| 🎣 Vara de pesca | 2× 🌲 Lenha, 1× 🪢 Corda, 1× 🪝 Anzol | 2 | — |
| 🌾 Sementes ×3 | 1× 🌽 Milho | 1 | — |
| 🧨 Bombinhas ×2 | 1× ⚫ Pólvora, 1× 🧵 Pano | 2 | — |
| 🪈 Cano de ferro | 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 2 | — |
| 🪤 Armadilha de urso | 2× 🔲 Chapa de metal, 3× 🔩 Sucata, 4× 📌 Prego | 3 | 🔨 martelo |
| 🛠️ Bancada de trabalho | 8× 📏 Tábua, 10× 📌 Prego, 3× 🔩 Sucata | 3 | 🔨 martelo |
| 🧥 Jaqueta de couro | 4× 🟫 Couro, 3× 🧵 Pano, 1× 🪢 Corda | 3 | — |
| 🦺 Colete improvisado | 6× 🧵 Pano, 2× 🔲 Chapa de metal, 2× 🧷 Fita adesiva, 2× 🪢 Corda | 4 |  🛠️ bancada |
| 🛡️ Colete balístico | 1× 🦺 Colete improvisado, 3× 🔲 Chapa de metal, 3× 🟫 Couro, 3× 🧷 Fita adesiva | 7 |  🛠️ bancada |
| 🔲 Chapa de metal | 5× 🔩 Sucata | 3 |  🛠️ bancada |
| 🔨 Marreta | 3× 🔲 Chapa de metal, 2× 🌲 Lenha, 1× 🧷 Fita adesiva | 5 |  🛠️ bancada |
| 🔸 Munição 9mm ×6 | 1× ⚫ Pólvora, 1× 🔩 Sucata | 5 |  🛠️ bancada |
| 🟥 Cartucho calibre 12 ×3 | 1× ⚫ Pólvora, 1× 🔩 Sucata, 1× 🧵 Pano | 5 |  🛠️ bancada |
| 💊 Antibiótico | 2× ⚗️ Produtos químicos, 1× 🧪 Álcool | 6 |  🛠️ bancada |
| 🔋 Bateria | 2× ➰ Fio de cobre, 1× ⚗️ Produtos químicos, 1× 🔩 Sucata | 6 |  🛠️ bancada |
| 🍳 Omelete | 2× 🥚 Ovo | 1 |  🔥 fogueira |
| 🥣 Sopa quente | 1× 🥫 Feijão enlatado, 1× 🫗 Água suja | 1 |  🔥 fogueira |
| 🍵 Chá de ervas | 1× 🫗 Água suja, 1× 🌿 Erva medicinal | 2 |  🔥 fogueira |
| 🍿 Pipoca ×2 | 1× 🌽 Milho | 1 |  🔥 fogueira |
| 🩻 Gaze estéril ×2 | 2× 🧵 Pano, 1× 🧪 Álcool | 3 | — |
| 🧴 Pomada cicatrizante ×2 | 2× 🌿 Erva medicinal, 1× 🧪 Álcool | 4 | — |
| 🏑 Clava de madeira | 3× 🌲 Lenha, 3× 📌 Prego | 1 | — |
| 🥊 Soco inglês | 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 3 |  🛠️ bancada |
| 🪏 Pá | 1× 🔲 Chapa de metal, 2× 🌲 Lenha, 2× 📌 Prego | 2 | 🔨 martelo |
| ⛏️ Picareta | 2× 🔲 Chapa de metal, 2× 🌲 Lenha, 1× 🧷 Fita adesiva | 4 |  🛠️ bancada |
| 🪓 Machado de incêndio | 1× 🪓 Machado, 2× 🔲 Chapa de metal, 2× 🧷 Fita adesiva | 6 |  🛠️ bancada |
| 🏹 Arco | 3× 🌲 Lenha, 2× 🪢 Corda | 3 | — |
| ➶ Flecha ×5 | 1× 🌲 Lenha, 1× 🔩 Sucata, 1× 🧵 Pano | 2 | — |
| ⛑️ Capacete de ciclista | 2× 🟫 Couro, 2× 🧵 Pano, 1× 🧷 Fita adesiva | 3 | — |
| 🪖 Capacete militar | 2× 🔲 Chapa de metal, 2× 🟫 Couro, 2× 🧷 Fita adesiva | 5 |  🛠️ bancada |
| 💥 Bomba caseira | 1× 🪈 Cano de ferro, 3× ⚫ Pólvora, 1× 🧷 Fita adesiva | 5 | — |
| 🌫️ Bomba de fumaça | 1× ⚫ Pólvora, 1× 🧵 Pano, 1× ⚗️ Produtos químicos | 4 | — |
| 🎒 Mochila de expedição | 1× 🎒 Mochila tática, 4× 🟫 Couro, 3× 🪢 Corda, 3× 🧷 Fita adesiva | 8 |  🛠️ bancada |
| 🍗 Frango assado | 1× 🍗 Frango cru | 1 |  🔥 fogueira |
| 🍞 Pão ×2 | 2× 🌾 Farinha, 1× 🫗 Água suja | 2 |  🔥 fogueira |
| 🔧 Chave inglesa | 1× 🔲 Chapa de metal, 2× 🔩 Sucata | 2 | — |
| 🏑 Cassetete | 2× 🌲 Lenha, 1× 🧷 Fita adesiva | 1 | — |
| 📯 Apito | 1× 🔲 Chapa de metal | 1 | — |
| 🧰 Caixa de ferramentas | 6× 🔩 Sucata, 2× 🔲 Chapa de metal | 3 | — |
| ⛽ Galão de gasolina | 2× 🔲 Chapa de metal, 3× ⛽ Combustível | 3 | — |
| 🛠️ Kit de reparo de veículo | 1× 🧰 Caixa de ferramentas, 4× 🔩 Sucata, 2× 🧷 Fita adesiva | 4 | — |
| 🦺 Colete de couro | 5× 🟫 Couro, 2× 🪢 Corda, 3× 🧵 Pano | 4 | — |
| ⚔️ Armadura de placas | 6× 🔲 Chapa de metal, 2× 🟫 Couro, 3× 🧷 Fita adesiva | 7 |  🛠️ bancada |
| 🪖 Capacete tático | 3× 🔲 Chapa de metal, 2× 🟫 Couro, 2× 🧷 Fita adesiva | 6 |  🛠️ bancada |
| 🔪 Cutelo | 2× 🔲 Chapa de metal, 1× 🌲 Lenha, 1× 🧷 Fita adesiva | 4 |  🛠️ bancada |
| 💧 Soro fisiológico ×2 | 1× 💧 Garrafa d’água, 1× 🧂 Sal | 3 | — |
| 💉 Esteroide de emergência | 1× 💉 Adrenalina, 1× 💊 Analgésico, 1× ⚗️ Produtos químicos | 7 |  🛠️ bancada |
| 🍜 Miojo pronto | 1× 🍜 Macarrão instantâneo, 1× 🫗 Água suja | 1 |  🔥 fogueira |
| 🥓 Bacon frito | 1× 🥓 Bacon cru | 1 |  🔥 fogueira |
| 🥩 Bife grelhado | 1× 🥩 Bife cru, 1× 🧂 Sal | 2 |  🔥 fogueira |
| 🥧 Torta de maçã | 2× 🍎 Maçã, 1× 🌾 Farinha, 1× 🍯 Mel | 3 |  🔥 fogueira |
| 🥪 Sanduíche | 1× 🍞 Pão, 1× 🧀 Queijo, 1× 🥓 Presunto fatiado | 1 | — |
| 🌭 Cachorro-quente | 1× 🍞 Pão, 1× 🌭 Salsicha em lata | 1 | — |
| 🍋 Limonada | 2× 🍋 Limão, 1× 🫗 Água suja, 1× 🍯 Mel | 1 | — |
| 🍵 Chá de ervas | 1× 🌿 Saquinho de ervas, 1× 🫗 Água suja | 1 |  🔥 fogueira |
| 🌿 Saquinho de ervas ×2 | 2× 🌿 Erva medicinal, 1× 🧵 Pano | 1 | — |
| 🧴 Xarope | 2× 🌿 Erva medicinal, 1× 🍯 Mel, 1× 🧪 Álcool | 3 | — |
| 🧪 Antídoto | 1× ⚗️ Produtos químicos, 2× 🌿 Erva medicinal, 1× 💧 Soro fisiológico | 5 | — |
| 🦴 Tala improvisada | 1× 📏 Tábua, 2× 🧵 Pano, 1× 🧷 Fita adesiva | 1 | — |
| 🧰 Maleta de primeiros socorros | 1× 🧰 Kit médico, 1× 💧 Soro fisiológico, 2× 🩻 Gaze estéril | 6 | — |
| 📏 Atiçador de ferro | 2× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 2 | — |
| 🔧 Chave de fenda | 1× 🔲 Chapa de metal, 1× 🧩 Plástico | 1 | — |
| 🏒 Taco de hóquei | 2× 🌲 Lenha, 1× 🧷 Fita adesiva | 1 | — |
| 🥋 Tonfa policial | 1× 📏 Tábua, 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 2 | — |
| 🔱 Maça de pregos | 1× 🏑 Clava de madeira, 6× 📌 Prego, 1× 🔲 Chapa de metal | 5 |  🛠️ bancada |
| 🔨 Martelo de guerra | 1× 🧱 Barra de aço, 2× 🌲 Lenha, 2× 🧷 Fita adesiva | 7 |  🛠️ bancada |
| 🌾 Foice | 3× 🔲 Chapa de metal, 2× 🌲 Lenha, 1× 🪢 Corda | 5 |  🛠️ bancada |
| 🗡️ Sabre | 1× 🧱 Barra de aço, 1× 🟫 Couro, 1× 🧷 Fita adesiva | 7 |  🛠️ bancada |
| 🔫 Espingarda de cano serrado | 1× 🔫 Espingarda de cano duplo, 1× 🧷 Fita adesiva, 1× 🔲 Chapa de metal | 6 |  🛠️ bancada |
| 🏹 Arco composto | 1× 🏹 Arco, 2× 🌀 Mola, 3× ➰ Fio de cobre, 1× 🧩 Plástico | 7 |  🛠️ bancada |
| 🔫 Mini submetralhadora | 1× 🔫 Submetralhadora, 2× 🌀 Mola, 1× 🧱 Barra de aço | 8 |  🛠️ bancada |
| ✨ Granada de luz | 1× 🔋 Bateria, 1× ⚫ Pólvora, 1× 🧩 Plástico | 4 |  🛠️ bancada |
| 🧨 Dinamite | 2× ⚫ Pólvora, 1× 🪢 Corda, 1× 🟡 Enxofre | 5 |  🛠️ bancada |
| ☄️ Bomba incendiária | 2× ⛽ Combustível, 1× 🧴 Cola forte, 1× 🍾 Garrafa vazia | 4 | — |
| 🧥 Moletom grosso | 3× 🧵 Tecido grosso, 2× 🧵 Pano | 2 | — |
| 🧥 Jaqueta de motoqueiro | 4× 🟫 Couro, 2× ⚫ Borracha, 2× 🧷 Fita adesiva | 5 | — |
| 🦺 Colete tático | 4× 🧵 Tecido grosso, 3× 🧩 Plástico, 1× 🧱 Barra de aço | 7 |  🛠️ bancada |
| 👷 Capacete de obra | 3× 🧩 Plástico, 1× 🧴 Cola forte | 2 | — |
| 🥽 Máscara de soldador | 1× 🔲 Chapa de metal, 1× 🧩 Plástico, 1× 🧴 Cola forte | 3 | — |
| 👝 Pochete | 1× 🧵 Tecido grosso, 1× 🪢 Corda | 1 | — |
| 👜 Mala esportiva | 4× 🧵 Tecido grosso, 2× 🪢 Corda, 1× 🧷 Fita adesiva | 3 | — |
| 🧴 Cola forte | 2× 🦴 Osso, 1× 💧 Garrafa d’água | 2 |  🔥 fogueira |
| 🌀 Mola ×2 | 2× ➰ Fio de cobre | 2 | — |
| 🟡 Enxofre | 1× ⚗️ Produtos químicos, 1× 🧂 Sal | 3 | — |
| 🧩 Plástico ×2 | 1× 🍾 Garrafa vazia | 1 | — |
| 🧱 Barra de aço | 3× 🔲 Chapa de metal, 2× 🔩 Sucata | 5 |  🛠️ bancada |
| 💾 Placa eletrônica | 1× 📻 Rádio de emergência | 3 | — |
| 🍄 Cogumelo assado | 1× 🍄 Cogumelo cru | 1 |  🔥 fogueira |
| 🌮 Taco | 1× 🌾 Farinha, 1× 🥩 Carne crua, 1× 🍅 Tomate | 2 |  🔥 fogueira |
| 🌯 Burrito | 1× 🌾 Farinha, 1× 🍚 Pacote de arroz, 1× 🍖 Carne assada | 3 |  🔥 fogueira |
| 🍢 Espetinho ×2 | 1× 🥩 Carne crua, 1× 🌲 Lenha | 1 |  🔥 fogueira |
| ☕ Chocolate quente | 1× 🍫 Chocolate, 1× 🥛 Leite longa vida | 1 |  🔥 fogueira |
| 🥤 Vitamina de frutas | 1× 🍌 Banana, 1× 🍒 Cerejas, 1× 🫗 Água suja | 1 | — |
| 🥛 Shake de proteína | 1× 🥛 Leite longa vida, 1× 🥚 Ovo, 1× 🍯 Mel | 2 | — |
| 🩹 Compressa estéril ×2 | 2× 🧵 Pano, 1× 🧪 Álcool | 2 | — |
| 🧪 Iodo antisséptico | 1× 🧪 Álcool, 1× 🧂 Sal, 1× 🌿 Erva medicinal | 3 | — |
| 🩺 Kit cirúrgico | 2× 🩹 Curativo, 2× 🩹 Compressa estéril, 1× 🔩 Sucata, 1× 🧪 Álcool | 6 | — |
| 📎 Grampos ×4 | 1× ➰ Fio de cobre | 1 | — |
| 🗝️ Gazua | 3× 📎 Grampos, 1× 🔲 Chapa de metal | 3 | — |
| 🧤 Luvas de trabalho | 2× 🟫 Couro, 2× 🧵 Pano | 2 | — |
| 🥾 Botas reforçadas | 3× 🟫 Couro, 2× ⚫ Borracha, 1× 🪢 Corda | 4 | — |
| 🪢 Mangueira | 2× ⚫ Borracha, 1× 🧷 Fita adesiva | 2 | — |
| 🔭 Binóculos | 2× 🧩 Plástico, 1× 🔲 Chapa de metal, 1× 🧴 Cola forte | 5 | — |
| 🟩 Lona ×2 | 3× 🧵 Tecido grosso, 1× 🧷 Fita adesiva | 1 | — |
| 🧰 Caixa de pregos | 12× 📌 Prego | 1 | — |
| 🔪 Faca de caco | 1× 🍾 Garrafa vazia, 1× 🧷 Fita adesiva | 1 | — |
| 📏 Vergalhão | 2× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 2 | — |
| 🦯 Bengala de ferro | 1× 🔲 Chapa de metal, 1× 🌲 Lenha, 1× 🧷 Fita adesiva | 2 | — |
| 🔱 Forcado | 2× 🌲 Lenha, 2× 🔲 Chapa de metal, 1× 🪢 Corda | 3 |  🛠️ bancada |
| 🪓 Machadinha | 1× 🪓 Machado, 1× 🧷 Fita adesiva, 1× 🔲 Chapa de metal | 4 |  🛠️ bancada |
| 🥋 Nunchaku | 2× 🌲 Lenha, 1× 🪢 Corda, 1× 🧷 Fita adesiva | 3 | — |
| 🗡️ Baioneta | 1× 🔪 Faca, 1× 🔲 Chapa de metal, 1× 🧷 Fita adesiva | 4 |  🛠️ bancada |
| 🔧 Pistola de pregos | 1× 🧰 Caixa de ferramentas, 2× 🌀 Mola, 1× 🔋 Bateria, 2× 🔲 Chapa de metal | 6 |  🛠️ bancada |
| 🔫 Pistola pesada | 1× 🔫 Pistola 9mm, 1× 🧱 Barra de aço, 1× 🌀 Mola | 6 |  🛠️ bancada |
| 🔫 Rifle de caça | 1× 🎯 Rifle, 1× 🧱 Barra de aço, 2× 🌀 Mola | 7 |  🛠️ bancada |
| 🔫 Submetralhadora MP5 | 1× 🔫 Submetralhadora, 1× 🧱 Barra de aço, 2× 🌀 Mola, 1× 🧩 Plástico | 8 |  🛠️ bancada |
| 🧥 Casaco longo | 4× 🧵 Tecido grosso, 1× 🟫 Couro, 1× 🧷 Fita adesiva | 3 | — |
| 🥼 Traje de proteção | 4× 🧩 Plástico, 2× 🟩 Lona, 3× 🧷 Fita adesiva, 2× ⚫ Borracha | 6 |  🛠️ bancada |
| 🛡️ Proteções esportivas | 3× 🧵 Tecido grosso, 3× 🧩 Plástico, 1× ⚫ Borracha | 3 | — |
| 😷 Máscara de gás | 2× ⚫ Borracha, 1× 🧩 Plástico, 2× 🧵 Pano | 4 | — |
| 🧢 Gorro de lã | 1× 🧵 Tecido grosso, 1× 🧵 Pano | 1 | — |
| 🪖 Capacete com viseira | 1× ⛑️ Capacete de ciclista, 2× 🧩 Plástico, 1× 🧴 Cola forte | 3 | — |
| 🎒 Mochila de acampamento | 2× 🟩 Lona, 3× 🧵 Tecido grosso, 2× 🪢 Corda | 4 | — |
| 🦺 Colete de bolsos | 2× 🧵 Tecido grosso, 1× 🪢 Corda, 2× 🧵 Pano | 2 | — |
| ⚙️ Peça de motor | 1× 🧱 Barra de aço, 2× ⚙️ Engrenagem, 1× 🛢️ Óleo de motor | 5 |  🛠️ bancada |
| 🛢️ Tambor de combustível | 2× ⛽ Galão de gasolina, 2× 🔲 Chapa de metal | 5 |  🛠️ bancada |
| 🤢 Bomba de fedor | 1× ⚗️ Produtos químicos, 1× 🍾 Garrafa vazia, 1× 🥩 Carne crua | 2 | — |
| 💨 Gás lacrimogêneo | 1× ⚗️ Produtos químicos, 1× 🟡 Enxofre, 1× 🧩 Plástico | 5 |  🛠️ bancada |


Fabricar dá XP de **Fabricação**, que também acelera a construção de barricadas.

## 12. Catálogo de itens

### Comida, bebida e remédios
| Item | Peso | Efeito |
| --- | --- | --- |
| 🥫 Feijão enlatado | 0.4 | +30 fome |
| 🍟 Salgadinho | 0.15 | +14 fome, -4 sede |
| 🍎 Maçã | 0.2 | +10 fome, +6 sede |
| 🍞 Pão | 0.3 | +22 fome |
| 💧 Garrafa d’água | 0.5 | +40 sede |
| 🥤 Refrigerante | 0.4 | +22 sede, +8 energia |
| 🩹 Curativo | 0.1 | +14 vida, estanca sangramento |
| 🧰 Kit médico | 1 | +60 vida, estanca sangramento |
| 💊 Antibiótico | 0.1 | -35 infecção, proteção temporária |
| 💉 Soro experimental | 0.2 | -100 infecção, proteção temporária |
| 🐟 Atum enlatado | 0.35 | +26 fome, -2 sede |
| 🥓 Carne seca | 0.2 | +34 fome, -6 sede |
| 🍫 Barra de cereal | 0.1 | +14 fome, +8 energia |
| 🍑 Pêssego em calda | 0.35 | +18 fome, +8 sede |
| 🍱 Ração militar | 0.5 | +55 fome, +8 sede, +10 energia |
| 🧃 Suco de caixinha | 0.3 | +28 sede, +6 fome |
| ⚡ Energético | 0.3 | +14 sede, +38 energia |
| ☕ Garrafa térmica de café | 0.5 | +8 sede, +26 energia |
| 💊 Analgésico | 0.05 | +22 vida |
| 🧴 Antisséptico | 0.2 | -15 infecção, estanca sangramento |
| 💉 Adrenalina | 0.1 | +15 vida, +60 energia |
| 🐟 Peixe cru | 0.4 | +14 fome |
| 🍣 Peixe assado | 0.35 | +40 fome, +4 sede |
| 🥩 Carne crua | 0.5 | +16 fome |
| 🍖 Carne assada | 0.45 | +52 fome, +4 energia |
| 🌽 Milho | 0.25 | +16 fome, +3 sede |
| 🍅 Tomate | 0.2 | +9 fome, +9 sede |
| 🥔 Batata | 0.3 | +14 fome |
| 🍲 Ensopado | 0.6 | +72 fome, +12 sede, +10 energia |
| 🍯 Mel | 0.3 | +20 fome, +14 energia |
| 🍫 Chocolate | 0.1 | +12 fome, +16 energia |
| 🍚 Pacote de arroz | 0.5 | +26 fome |
| 🫗 Água suja | 0.5 | +26 sede |
| 🟡 Vitaminas | 0.05 | +30 energia, +8 vida, proteção temporária |
| 🌿 Erva medicinal | 0.1 | +16 vida, estanca sangramento |
| 🍝 Macarrão | 0.4 | +24 fome |
| 🐟 Sardinha enlatada | 0.2 | +20 fome, +3 energia |
| 🥜 Pasta de amendoim | 0.4 | +26 fome, +8 energia |
| 🌰 Castanhas | 0.15 | +12 fome, +8 energia |
| 🍪 Biscoito | 0.1 | +10 fome, +4 energia |
| 🌭 Salsicha em lata | 0.3 | +28 fome |
| 🥣 Sopa quente | 0.5 | +46 fome, +14 sede, +6 energia |
| 🥚 Ovo | 0.1 | +8 fome |
| 🍳 Omelete | 0.3 | +38 fome, +6 energia |
| 🍿 Pipoca | 0.15 | +18 fome, -4 sede |
| 🥛 Leite longa vida | 0.5 | +26 sede, +10 fome |
| 🍵 Chá de ervas | 0.3 | +30 sede, +6 vida, +8 energia |
| 🍺 Cerveja | 0.4 | +10 sede, +6 fome, -6 energia |
| 🩻 Gaze estéril | 0.1 | +22 vida, estanca sangramento |
| 🧴 Pomada cicatrizante | 0.1 | +10 vida, estanca sangramento, -8 infecção |
| 🥓 Presunto fatiado | 0.3 | +22 fome |
| 🧀 Queijo | 0.3 | +24 fome |
| 🥣 Iogurte | 0.3 | +14 fome, +10 sede |
| 🍓 Geleia | 0.3 | +16 fome, +10 energia |
| 🍽️ Lasanha congelada | 0.6 | +58 fome, +6 energia |
| 🍔 Hambúrguer | 0.35 | +44 fome |
| 🍮 Pudim | 0.3 | +20 fome, +12 energia |
| 🥗 Salada pronta | 0.4 | +18 fome, +12 sede |
| 🍗 Frango cru | 0.6 | +15 fome |
| 🍗 Frango assado | 0.5 | +56 fome, +5 energia |
| 🥤 Refrigerante 2L | 1 | +44 sede, +14 energia |
| 🍷 Vinho | 0.7 | +8 sede, +6 fome, -10 energia, +6 vida |
| 🧃 Isotônico | 0.5 | +36 sede, +20 energia |
| 🥥 Água de coco | 0.6 | +34 sede, +8 fome |
| 💧 Soro fisiológico | 0.3 | +12 vida, -6 infecção |
| 💊 Antiviral | 0.1 | -60 infecção, proteção temporária |
| 💉 Esteroide de emergência | 0.1 | +35 vida, +45 energia |
| 🍕 Pizza congelada | 0.7 | +46 fome, +4 energia |
| 🥪 Sanduíche | 0.35 | +34 fome |
| 🌭 Cachorro-quente | 0.3 | +30 fome |
| 🍩 Rosquinha | 0.15 | +16 fome, +10 energia |
| 🍰 Fatia de bolo | 0.3 | +26 fome, +14 energia |
| 🍦 Sorvete | 0.3 | +12 fome, +8 sede, +8 energia |
| 🍌 Banana | 0.2 | +14 fome, +6 energia |
| 🍊 Laranja | 0.25 | +10 fome, +10 sede, +2 vida |
| 🍇 Uvas | 0.25 | +10 fome, +8 sede |
| 🍜 Miojo pronto | 0.5 | +42 fome, +6 sede |
| 🥓 Bacon cru | 0.3 | +10 fome |
| 🥓 Bacon frito | 0.25 | +34 fome, +4 energia |
| 🥩 Bife cru | 0.6 | +14 fome |
| 🥩 Bife grelhado | 0.5 | +62 fome, +8 energia |
| 🥧 Torta de maçã | 0.6 | +40 fome, +10 energia |
| 🍋 Limonada | 0.5 | +38 sede, +6 energia |
| 🧋 Chá gelado | 0.5 | +34 sede, +8 energia |
| 🥛 Milkshake | 0.5 | +20 sede, +22 fome |
| 🍸 Vodca | 0.7 | -4 sede, -12 energia, +4 vida |
| 💦 Água com gás | 0.5 | +40 sede |
| 🍵 Chá de ervas | 0.4 | +24 sede, +10 vida, -8 infecção |
| 💊 Ibuprofeno | 0.05 | +8 vida, +12 energia |
| 🧴 Xarope | 0.3 | +10 vida, -14 infecção |
| 🧰 Maleta de primeiros socorros | 1.5 | +80 vida, estanca sangramento, -20 infecção |
| 💉 Morfina | 0.1 | +45 vida, estanca sangramento, -15 energia |
| 🧪 Antídoto | 0.1 | -40 infecção, +15 vida, proteção temporária |
| 🦴 Tala improvisada | 0.5 | +22 vida, estanca sangramento |
| 🌮 Taco | 0.3 | +32 fome |
| 🌯 Burrito | 0.45 | +44 fome, +4 energia |
| 🍢 Espetinho | 0.35 | +30 fome, +3 energia |
| 🍉 Melancia | 1.2 | +18 fome, +30 sede |
| 🍒 Cerejas | 0.15 | +8 fome, +6 sede, +4 energia |
| 🥕 Cenoura | 0.2 | +12 fome, +2 vida |
| 🥐 Croissant | 0.15 | +20 fome, +4 energia |
| 🥯 Bagel | 0.2 | +24 fome |
| 🥧 Torta doce | 0.4 | +30 fome, +12 energia |
| 🍄 Cogumelo cru | 0.1 | +6 fome |
| 🍄 Cogumelo assado | 0.1 | +22 fome, +3 energia |
| ☕ Chocolate quente | 0.4 | +22 sede, +8 fome, +10 energia |
| 🥛 Shake de proteína | 0.5 | +14 sede, +14 fome, +20 energia, +4 vida |
| 💧 Água mineral | 0.5 | +42 sede |
| 🥤 Vitamina de frutas | 0.5 | +28 sede, +12 fome, +3 vida |
| 🩺 Kit cirúrgico | 1.2 | +75 vida, estanca sangramento, -10 infecção |
| 🩹 Compressa estéril | 0.1 | +18 vida, estanca sangramento, -4 infecção |
| 🍊 Vitamina C | 0.05 | +4 vida, -10 infecção, +6 energia |
| 🧪 Iodo antisséptico | 0.2 | -28 infecção, +3 vida |


### Armas corpo a corpo
(ver tabela na seção 4)

### Armas de fogo
(ver tabela na seção 4)

### Armaduras
| Armadura | Peso | Redução de dano | Observação |
| --- | --- | --- | --- |
| 🧥 Jaqueta de couro | 1.4 | 14% | Armadura leve: -14% de dano recebido. |
| 🦺 Colete improvisado | 3 | 26% | Armadura média: -26% de dano recebido. |
| 🛡️ Colete balístico | 3.5 | 40% | Armadura pesada: -40% de dano recebido. |
| 🥋 Traje antimotim | 6 | 52% | Muito raro: -52% de dano, mas você anda um pouco mais devagar. |
| 🦺 Colete de couro | 2.2 | 20% | Armadura leve-média: −20% de dano. |
| ⚔️ Armadura de placas | 5.5 | 36% | Placas de aço: −36% de dano, um pouco pesada. |
| 🧥 Moletom grosso | 1 | 9% | Aquece e protege um pouco: −9% de dano. |
| 🧥 Jaqueta de motoqueiro | 2.8 | 27% | Couro com proteções: −27% de dano. |
| 🦺 Colete tático | 3.8 | 40% | Muito resistente: −40% de dano. |
| 🧥 Casaco longo | 1.6 | 16% | Tecido grosso: −16% de dano. |
| 🥼 Traje de proteção | 3 | 28% | −28% de dano e a infecção é bem mais difícil. |
| 🛡️ Proteções esportivas | 2 | 20% | Joelheiras e coletes: −20% de dano. |


### Materiais, munição, ferramentas e utilitários
| Item | Peso | Para que serve |
| --- | --- | --- |
| 🧵 Pano | 0.1 | Material para curativos. |
| 🌲 Lenha | 0.8 | Para fogueiras e tábuas. |
| 📏 Tábua | 0.7 | Usada em barricadas e baús. |
| 📌 Prego | 0.02 | Usado em barricadas. |
| 🔩 Sucata | 0.3 | Metal para fabricação. |
| 🔸 Munição 9mm | 0.02 | Para a pistola. |
| 🟥 Cartucho calibre 12 | 0.05 | Para a espingarda. |
| 🔶 Munição 7.62 | 0.03 | Para o rifle. |
| 🔦 Lanterna | 0.4 | Basta carregar: aumenta muito sua visão à noite. |
| 🎒 Mochila escolar | 0.8 | +6 espaços, +8 kg. |
| 🎒 Mochila militar | 1.2 | +12 espaços, +18 kg. |
| 🏕️ Fogueira | 3 | Ilumina, cura mais rápido e queima zumbis próximos. |
| 🧳 Baú | 6 | Guarde itens no abrigo. |
| 📢 Isca sonora | 0.3 | Joga um som à frente e atrai zumbis para lá. |
| 🗝️ Chave do bunker | 0.1 | Abre o bunker militar. |
| 🪢 Corda | 0.4 | Para fabricar mochilas e armas. |
| 🧷 Fita adesiva | 0.1 | Prende e conserta de tudo. |
| 🔲 Chapa de metal | 1 | Material pesado e resistente. |
| 🍾 Garrafa vazia | 0.3 | Pode virar um molotov. |
| ⚫ Pólvora | 0.1 | Usada em explosivos caseiros. |
| 🔹 Munição .357 | 0.03 | Para o revólver. |
| 🔻 Virote | 0.04 | Para a besta. |
| 🎒 Mochila de trilha | 1 | +9 espaços, +13 kg. |
| 🎒 Mochila tática | 1.6 | +18 espaços, +28 kg. Rara. |
| 🔥 Coquetel molotov | 0.5 | Joga à frente e cria um incêndio. Queima zumbis. |
| 💣 Granada caseira | 0.5 | Explode 2 segundos depois. Cuidado com o próprio alcance! |
| 🧪 Álcool | 0.3 | Desinfeta. Usado em antissépticos. |
| 🧱 Parede de madeira | 1.2 | Modo de construção: escolha qualquer quadrado da grade. Com o martelo equipado, Usar desmonta. |
| 🚪 Portão de madeira | 1.5 | Porta que você posiciona onde quiser. |
| 🛏️ Cama de abrigo | 4 | Posicione e ofereça abrigo: sobreviventes podem se mudar para ela (modo offline). |
| 🌱 Muda de árvore | 0.2 | Plante em grama, terra ou toco. Vira árvore em alguns minutos. |
| 🗺️ Mapa da região | 0.1 | Use para revelar uma grande área do mapa ao redor. |
| 🌾 Sementes | 0.05 | Plante em terra ou grama (modo de construção). Crescem em alguns minutos e rendem comida. |
| 🟫 Couro | 0.4 | Material para armaduras. |
| 🦴 Osso | 0.2 | Resto de caça. |
| 🔋 Bateria | 0.3 | Alimenta o rádio. |
| ➰ Fio de cobre | 0.2 | Material eletrônico. |
| ⚗️ Produtos químicos | 0.3 | Base de remédios e explosivos. |
| ⚙️ Engrenagem | 0.4 | Peça mecânica. |
| 🪝 Anzol | 0.02 | Para varas de pesca. |
| 🎣 Vara de pesca | 0.8 | Tenha na mochila e use perto da água para pescar. |
| 📻 Rádio de emergência | 1 | Gasta 1 bateria e chama um lançamento de suprimentos no local onde você estiver. |
| 🪤 Armadilha de urso | 2 | Posicione no chão: prende e fere quem pisar (zumbis e você!). Rearme com Usar. |
| 🛠️ Bancada de trabalho | 6 | Fique perto dela para fabricar itens avançados. |
| 🧨 Bombinhas | 0.2 | Joga à frente e faz um estouro enorme: atrai zumbis para lá. |
| ➶ Flecha | 0.03 | Para o arco. |
| 💥 Bomba caseira | 0.8 | Explosão dupla muito mais forte que a granada. |
| 🌫️ Bomba de fumaça | 0.4 | Desorienta os zumbis num raio grande por alguns segundos. |
| 🎒 Mochila de expedição | 2 | +24 espaços, +40 kg. Rara. |
| 🧂 Sal | 0.2 | Conserva e tempera. |
| 🌾 Farinha | 0.5 | Para fazer pão na fogueira. |
| 📯 Apito | 0.1 | Joga um som à frente e atrai zumbis para lá. |
| 🧰 Caixa de ferramentas | 2.5 | Cheia de peças úteis. Usada em receitas avançadas. |
| 🍜 Macarrão instantâneo | 0.2 | Cozinhe numa fogueira com água. |
| ✨ Granada de luz | 0.4 | Atordoa zumbis num raio grande por um bom tempo. Faz barulho. |
| 🧨 Dinamite | 0.6 | Três explosões seguidas. Perigosíssima. |
| ☄️ Bomba incendiária | 0.8 | Espalha um grande mar de fogo. |
| 👝 Pochete | 0.3 | +3 espaços, +4 kg. |
| 👜 Mala esportiva | 1.8 | +14 espaços, +22 kg. |
| 🧴 Cola forte | 0.2 | Para reforçar peças e armas. |
| 🌀 Mola | 0.1 | Peça de mecanismo. |
| ⚫ Borracha | 0.4 | Pedaços de pneu e mangueira. |
| 🧩 Plástico | 0.2 | Reciclável e leve. |
| 🟡 Enxofre | 0.3 | Para pólvora e bombas. |
| 🧲 Ímã | 0.2 | Útil em eletrônicos. |
| 💾 Placa eletrônica | 0.2 | Para rádios e aparelhos. |
| 🧱 Barra de aço | 1.5 | Base de armas e armaduras pesadas. |
| 🧵 Tecido grosso | 0.3 | Lona e brim resistentes. |
| 🌿 Saquinho de ervas | 0.2 | Para chás e remédios caseiros. |
| 🍋 Limão | 0.15 | Para limonada ou cozinhar. |
| 🎒 Mochila de acampamento | 1.5 | +16 espaços, +28 kg. |
| 🦺 Colete de bolsos | 0.9 | +7 espaços, +10 kg. Leve. |
| 🗝️ Gazua | 0.1 | Tenha na mochila: abre portas trancadas em silêncio (chance depende de Garimpo). Pode quebrar. |
| 🧤 Luvas de trabalho | 0.2 | Tenha na mochila: evita cortes ao quebrar vidro e pisar em cacos. |
| 🥾 Botas reforçadas | 1.2 | Tenha na mochila: menos dano de armadilhas e menos cortes por cacos. |
| 🪢 Mangueira | 0.4 | Tenha na mochila: permite sifonar combustível de veículos parados. |
| 🔭 Binóculos | 0.5 | Tenha na mochila: enxerga um pouco mais longe à noite. |
| 🤢 Bomba de fedor | 0.4 | Libera um barulho enorme por vários segundos e atrai zumbis para longe de você. |
| 💨 Gás lacrimogêneo | 0.5 | Nuvem que atordoa e fere zumbis por ~10 s num raio médio. |
| 📎 Grampos | 0.02 | Para fazer gazuas. |
| ⚫ Pneu | 4 | Borracha pesada. Útil para trabalhos de oficina. |
| 🟩 Lona | 0.8 | Cobertura resistente. |
| 🛢️ Óleo de motor | 1 | Lubrifica e queima bem. |
| 🧰 Caixa de pregos | 0.8 | Pregos soltos e fáceis de usar como munição. |


## 13. Progressão

Tudo que você faz dá **XP**. Ao subir de nível você ganha **2 pontos de atributo**.

### Atributos (Perfil)
| Atributo | Efeito por ponto |
| --- | --- |
| **Força** | +4% de dano corpo a corpo e +2 kg de carga |
| **Vitalidade** | +8 de vida máxima, −2% de dano recebido, −3% de chance de infecção |
| **Agilidade** | +2,5% de velocidade |

### Habilidades (evoluem usando)
| Habilidade | Efeito |
| --- | --- |
| 🗡️ **Combate corpo a corpo** | +8% de dano por nível |
| 🎯 **Precisão (armas de fogo)** | −5% de dispersão e recarga mais rápida |
| 🔍 **Coleta de recursos** | Revista mais rápido e acha mais itens |
| 🔨 **Fabricação** | Libera receitas e acelera construção |
| 🏃 **Resistência física** | Mais fôlego e corrida mais veloz |
| 🥷 **Furtividade** | −6% de ruído por nível |
| 🏕️ **Sobrevivência** | Pesca, colheita e caça rendem mais e mais rápido; menos enjoo com comida crua |

## 14. Missões

Abra com **J** (ou pelo menu). Cumprir uma missão dá XP e recompensa.

| Missão | Objetivo | Recompensa |
| --- | --- | --- |
| Primeiros cuidados | Comer ou beber 2 vezes | 2 curativos |
| Catador | Revistar 6 recipientes | comida e água |
| Abrigo seguro | Barricar uma porta ou janela | tábuas e pregos |
| Mãos à obra | Fabricar 3 itens | sucata e panos |
| Limpeza de área | Abater 10 zumbis | munição 9mm |
| Plantão | Explorar o hospital | kit médico e antibiótico |
| Lei e ordem | Entrar na delegacia (porta trancada) | munição |
| Caçada ao Gritador | Derrotar o Gritador | kit médico |
| Segredo militar | Abrir o bunker com a chave do Gritador | soro experimental |
| Sobrevivente | Chegar ao dia 4 | mochila militar |
| Entrada discreta | Quebrar 3 janelas | panos e fita |
| Pescador | Pescar 3 peixes | anzóis e corda |
| Chef de fogueira | Cozinhar 3 receitas na fogueira | arroz e carne seca |
| Mãos na terra | Colher 2 plantações | sementes e batatas |
| Blindado | Vestir uma armadura | curativos e vitamina |
| Oficina | Fabricar 2 itens na bancada | metal e engrenagens |
| Armadilheiro | Abater 2 zumbis com armadilhas | metal e armadilha |
| Caçador | Caçar 3 animais (offline) | armadilha e couro |
| Sinal de socorro | Usar o rádio ao ar livre | bateria e comida |
| Cientista maluco | Explorar o laboratório | soro experimental |
| Demolidor | Derrubar 3 paredes | metal e fita |
| Mãos leves | Abrir 2 portas trancadas com gazua | grampos e luvas |
| Sombra silenciosa | 3 mortes com golpe furtivo | apito e gorro |
| Ladrão de gasolina | Sifonar combustível de um veículo | galão |
| Duas rodas | Dirigir uma moto | capacete de moto |
| Peso pesado | Dirigir um caminhão | peça de motor |
| Ao volante | Entrar num veículo | galão de gasolina |
| Atropelador | Atropelar 8 zumbis | kit de reparo e capacete |
| Mecânico de campo | Consertar um veículo | caixa de ferramentas e chave inglesa |
| Dia de compras | Entrar num shopping | mochila de trilha e jaqueta |
| Veterano | Chegar ao dia 8 | colete balístico |

As missões que dependem de um local mostram a direção (ex.: "ao norte").

## 15. Dia, noite, clima e eventos

- **Um dia dura cerca de 12 minutos reais.** Dormindo, o tempo passa bem mais rápido.
- **Noite:** a tela escurece e a visão cai. A **lanterna** ajuda; fogueiras iluminam.
- **Clima:** 🌧 **chuva** abafa seus passos; 🌫 **neblina** reduz a visão (sua e dos zumbis).
- **Eventos:** helicópteros podem largar suprimentos 🚁 (ponto dourado no mapa) e, a partir do dia 2, **hordas** podem se formar nas ruas (ponto vermelho no mapa).
- **Dificuldade cresce:** a cada dia surgem mais corredores e tanques, e zumbis novos aparecem.

## 16. Modo celular

- **Tela cheia real** (API de Fullscreen) e **bloqueio de orientação horizontal**; se o navegador não permitir o bloqueio, aparece o aviso para **girar o aparelho manualmente**.
- Interface adaptada à horizontal: joystick à esquerda, botões à direita, minimapa no canto.
- **Gestos acidentais** (voltar, zoom, rolagem, menu de contexto) são bloqueados.
- Ao trocar de app ou sair da tela cheia, o jogo **pausa e salva**; ao voltar você continua de onde parou.
- Se tela cheia ou bloqueio de orientação não estiverem disponíveis, o jogo **continua funcionando normalmente**.
- Em **Opções** você escolhe o modo de toque (automático, ligado, desligado), vibração, auto-mira e volumes.

## 17. Salvamento

- O jogo **salva sozinho** a cada poucos segundos e sempre que você sai, troca de app ou pausa. O save fica no **navegador** (localStorage), neste aparelho.
- **Morreu no solo = save apagado.** Comece de novo pelo menu.
- Saves antigos do **mapa menor** (versão anterior) continuam abrindo normalmente no mapa antigo; novos jogos usam o mapa grande.
- Limpar os dados do navegador apaga o save.

## 18. Co-op online

Até **8 jogadores** no mesmo mundo. O **anfitrião** roda o mundo e os zumbis no próprio navegador; os outros entram com um **código de 4 letras**.

#### 🛡️ Modo sem fogo amigo (dispersão)
Ao **criar a sala**, marque **"Modo sem fogo amigo"**. Nesse modo:
- **Explosões lançadas por aliados não ferem você** (granada, bomba caseira, dinamite). Quem lança ainda se machuca com a própria explosão; barris e carros explodindo continuam perigosos para todos.
- **Cada jogador nasce em um lugar diferente do mapa**, longe dos outros (dezenas de quarteirões) e sem zumbis por perto. Ao renascer você volta ao seu ponto de origem.
- Sem a opção marcada, o co-op funciona como antes: todos nascem juntos no abrigo e as explosões ferem quem estiver perto, aliado ou não.
- Armas de fogo e golpes corpo a corpo **nunca** ferem aliados em nenhum modo.

1. Menu → **🌐 Online**.
2. Digite seu nome. Se você abriu o jogo de outro endereço que não o do servidor (por exemplo, GitHub Pages), preencha o campo **Servidor** com o endereço do seu servidor, como `wss://seu-nome.onrender.com`.
3. **Criar sala** (anfitrião) ou digite o **código** e toque em **Entrar**. Dá para copiar o link da sala para enviar aos amigos.

O que funciona no co-op: mundo, zumbis, portas, baús, loot, barricadas, **construções (paredes, portões, camas, mudas)**, explosões e dano. Cada jogador tem inventário e progresso próprios; jogadores aliados aparecem no mapa.

Limitações:
- O anfitrião precisa **manter a aba aberta e a tela ligada**; se ele sair, a sala fecha.
- **Sem NPCs** nem **animais de caça** no online.
- Veículos: motorista + 3 passageiros, para anfitrião e convidados (a direção do convidado tem um pequeno atraso da rede). Armadilhas só disparam para o anfitrião ao pisar.
- Sem proteção contra trapaça (a detecção de acertos é feita em cada jogador).
- Se o servidor gratuito estava dormindo, a primeira conexão pode levar cerca de **1 minuto** (o jogo avisa e espera).
- Ao morrer no co-op você **renasce** no abrigo com um personagem novo.

## 19. Publicar o jogo

O jogo é um arquivo HTML estático e o servidor é um programa Node pequeno. Dá para separar os dois:

### Site do jogo (GitHub Pages)
1. Crie um repositório **público** só com o `index.html` (pasta `jogo/` do pacote).
2. *Settings → Pages →* Deploy from a branch (`main`, pasta `/root`).
3. O endereço será `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

### Servidor co-op (Render, plano gratuito)
1. Crie outro repositório com `server.js`, `package.json` e `render.yaml` (pasta `servidor/`). Pode ser **privado**.
2. No Render: **New → Web Service**, conecte o repositório. *Runtime:* Node · *Build:* `npm install` · *Start:* `npm start` · *Plano:* Free.
3. Teste `https://SEU-SERVICO.onrender.com/healthz`: deve mostrar `ok`.
4. No jogo, em **Online → Servidor**, use `wss://SEU-SERVICO.onrender.com`.
5. (Opcional) defina `ALLOWED_ORIGINS` no Render com o endereço do seu site para só ele usar o servidor.

**Variáveis do servidor:** `PORT`, `MAX_PLAYERS` (padrão 4), `MAX_ROOMS`, `ALLOWED_ORIGINS`.

**Manter o servidor gratuito acordado:** o plano gratuito dorme depois de ~15 min sem tráfego. O jogo envia um *ping* ao servidor ao criar/entrar numa sala e **a cada 10 minutos** enquanto você está online. A primeira conexão após um período dormindo pode demorar cerca de 1 minuto.

## 20. Dicas de sobrevivência

- **Comece pelo baú do abrigo:** pegue martelo, tábuas, pregos e panos. Barricar a porta é a primeira missão e te protege.
- **Revistar com calma:** faça isso longe de grupos de zumbis. Cada revista faz barulho.
- **Casas primeiro**, depois lojas. Hospital e delegacia só quando estiver bem armado.
- **Machado cedo:** lenha vira tábuas e fogueiras, e as mudas deixam a floresta renovável.
- **Corra só quando precisar:** o fôlego acaba e o barulho atrai zumbis.
- **Besta e facão** para economizar tiros; **molotov** e **granada** contra grupos.
- **Tome antibiótico logo** após uma mordida. Guarde o **soro** para emergência.
- **À noite**, fique no abrigo: durma, cozinhe na fogueira e organize o baú.
- **Construa dentro da casa ou num lote vazio**, com portão voltado para onde você vigia, e uma cama extra para atrair um sobrevivente.
- **Barris vermelhos** são armas: puxe os zumbis até eles e atire de longe.
- **Gritador:** mate-o longe de outros zumbis (o grito atrai todos) e pegue a **chave do bunker**.
- **Cerque o abrigo de armadilhas** (e lembre onde estão!). Uma **fazenda** ao lado da casa, uma **vara de pesca** e uma fogueira garantem comida sem sair à rua.
- **Pano + janela**: entre em prédios sem alarde quebrando o vidro com um pano; depois agache sobre os cacos.
- **Bancada cedo**: coletes e munição caseira mudam o jogo. Armazéns e lojas de ferragens têm material.
- **Ouro do laboratório**: químicos e baterias (com o rádio) valem o risco — mas leve armadura.
- **Um carro muda tudo no mapa de 992×992:** ache um perto do início, abasteça e use as ruas retas. Leve galão extra e um kit de reparo.
- Cuidado ao **parar o carro no meio de uma horda**: zumbis batem na lataria. Saia pelo lado livre (você desce ao lado do carro).
- Use o **mapa** para marcar o que já revistou e para achar suprimentos largados por helicópteros.

## 21. Problemas comuns

| Problema | Solução |
| --- | --- |
| Sem som | Toque na tela uma vez (navegadores exigem um toque antes de tocar áudio). Confira os volumes em Opções. |
| Tela cheia não abre | Alguns navegadores bloqueiam; no iPhone use *Adicionar à Tela de Início*. O jogo funciona sem tela cheia. |
| Aviso "gire o celular" | Gire o aparelho para horizontal; o jogo continua de onde parou. |
| Perdi meu save | Saves ficam no navegador do aparelho; limpar dados do site ou morrer (no solo) apaga. |
| Online: "Sala cheia" | O limite é 8 jogadores por sala (configurável no servidor com `MAX_PLAYERS`, 2 a 8). |
| Online: demora a conectar | O servidor gratuito estava dormindo. Aguarde até ~1 minuto. |
| Online: "O anfitrião saiu" | A sala fecha quando o anfitrião sai; crie outra. |
| Nenhum sobrevivente aparece | Só no modo offline. Você precisa de uma **cama sua** e algumas paredes/portões; camas de casas do mapa não contam. |
| Não consigo colocar um item | Quadrado vermelho: tem algo no lugar, está longe demais, é rua ou água. |
| Desempenho ruim no celular | Feche outras abas e apps; o jogo é leve, mas o mapa é grande. |

---

*Feito em HTML, CSS e JavaScript puros (Canvas 2D), sem bibliotecas externas. O co-op usa um servidor Node com WebSocket.*
