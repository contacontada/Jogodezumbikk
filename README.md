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
10. [Fabricação](#10-fabricação)
11. [Catálogo de itens](#11-catálogo-de-itens)
12. [Progressão: nível, atributos e habilidades](#12-progressão)
13. [Missões](#13-missões)
14. [Dia, noite, clima e eventos](#14-dia-noite-clima-e-eventos)
15. [Modo celular](#15-modo-celular)
16. [Salvamento](#16-salvamento)
17. [Co-op online](#17-co-op-online)
18. [Publicar o jogo (GitHub Pages + Render)](#18-publicar-o-jogo)
19. [Dicas de sobrevivência](#19-dicas-de-sobrevivência)
20. [Problemas comuns](#20-problemas-comuns)

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

O mapa é uma cidade grande (176×176 quadrados) com ruas, quarteirões, florestas, parques e lagos. Os locais mais importantes são marcados no mapa quando você os descobre:

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
| 🏚 **Bunker militar** | Trancado com a **chave do Gritador**. O melhor saque do jogo. |

- **Revistar** (E): armários, geladeiras, caixotes, mochilas abandonadas, porta-malas de carros. Leva alguns segundos e faz um pouco de barulho. Depois de revistado, o recipiente pode ser reaberto livremente.
- 🚁 **Helicópteros** podem largar caixas de suprimentos (aparecem no mapa como pontos dourados).
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

Fabrique os itens de construção (veja a [tabela](#10-fabricação)): 🧱 **parede de madeira**, 🚪 **portão de madeira**, 🛏️ **cama de abrigo**, além de 🧳 **baú** e 🔥 **fogueira**.

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

## 10. Fabricação

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


Fabricar dá XP de **Fabricação**, que também acelera a construção de barricadas.

## 11. Catálogo de itens

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


### Armas corpo a corpo
(ver tabela na seção 4)

### Armas de fogo
(ver tabela na seção 4)

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
| ⛽ Combustível | 0.8 | Inflamável. Base de molotovs. |
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


## 12. Progressão

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

## 13. Missões

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

As missões que dependem de um local mostram a direção (ex.: "ao norte").

## 14. Dia, noite, clima e eventos

- **Um dia dura cerca de 12 minutos reais.** Dormindo, o tempo passa bem mais rápido.
- **Noite:** a tela escurece e a visão cai. A **lanterna** ajuda; fogueiras iluminam.
- **Clima:** 🌧 **chuva** abafa seus passos; 🌫 **neblina** reduz a visão (sua e dos zumbis).
- **Eventos:** helicópteros podem largar suprimentos 🚁 (ponto dourado no mapa) e, a partir do dia 2, **hordas** podem se formar nas ruas (ponto vermelho no mapa).
- **Dificuldade cresce:** a cada dia surgem mais corredores e tanques, e zumbis novos aparecem.

## 15. Modo celular

- **Tela cheia real** (API de Fullscreen) e **bloqueio de orientação horizontal**; se o navegador não permitir o bloqueio, aparece o aviso para **girar o aparelho manualmente**.
- Interface adaptada à horizontal: joystick à esquerda, botões à direita, minimapa no canto.
- **Gestos acidentais** (voltar, zoom, rolagem, menu de contexto) são bloqueados.
- Ao trocar de app ou sair da tela cheia, o jogo **pausa e salva**; ao voltar você continua de onde parou.
- Se tela cheia ou bloqueio de orientação não estiverem disponíveis, o jogo **continua funcionando normalmente**.
- Em **Opções** você escolhe o modo de toque (automático, ligado, desligado), vibração, auto-mira e volumes.

## 16. Salvamento

- O jogo **salva sozinho** a cada poucos segundos e sempre que você sai, troca de app ou pausa. O save fica no **navegador** (localStorage), neste aparelho.
- **Morreu no solo = save apagado.** Comece de novo pelo menu.
- Saves antigos do **mapa menor** (versão anterior) continuam abrindo normalmente no mapa antigo; novos jogos usam o mapa grande.
- Limpar os dados do navegador apaga o save.

## 17. Co-op online

Até **4 jogadores** no mesmo mundo. O **anfitrião** roda o mundo e os zumbis no próprio navegador; os outros entram com um **código de 4 letras**.

1. Menu → **🌐 Online**.
2. Digite seu nome. Se você abriu o jogo de outro endereço que não o do servidor (por exemplo, GitHub Pages), preencha o campo **Servidor** com o endereço do seu servidor, como `wss://seu-nome.onrender.com`.
3. **Criar sala** (anfitrião) ou digite o **código** e toque em **Entrar**. Dá para copiar o link da sala para enviar aos amigos.

O que funciona no co-op: mundo, zumbis, portas, baús, loot, barricadas, **construções (paredes, portões, camas, mudas)**, explosões e dano. Cada jogador tem inventário e progresso próprios; jogadores aliados aparecem no mapa.

Limitações:
- O anfitrião precisa **manter a aba aberta e a tela ligada**; se ele sair, a sala fecha.
- **Sem NPCs** no online.
- Sem proteção contra trapaça (a detecção de acertos é feita em cada jogador).
- Se o servidor gratuito estava dormindo, a primeira conexão pode levar cerca de **1 minuto** (o jogo avisa e espera).
- Ao morrer no co-op você **renasce** no abrigo com um personagem novo.

## 18. Publicar o jogo

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

## 19. Dicas de sobrevivência

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
- Use o **mapa** para marcar o que já revistou e para achar suprimentos largados por helicópteros.

## 20. Problemas comuns

| Problema | Solução |
| --- | --- |
| Sem som | Toque na tela uma vez (navegadores exigem um toque antes de tocar áudio). Confira os volumes em Opções. |
| Tela cheia não abre | Alguns navegadores bloqueiam; no iPhone use *Adicionar à Tela de Início*. O jogo funciona sem tela cheia. |
| Aviso "gire o celular" | Gire o aparelho para horizontal; o jogo continua de onde parou. |
| Perdi meu save | Saves ficam no navegador do aparelho; limpar dados do site ou morrer (no solo) apaga. |
| Online: "Sala cheia" | O limite é 4 jogadores por sala. |
| Online: demora a conectar | O servidor gratuito estava dormindo. Aguarde até ~1 minuto. |
| Online: "O anfitrião saiu" | A sala fecha quando o anfitrião sai; crie outra. |
| Nenhum sobrevivente aparece | Só no modo offline. Você precisa de uma **cama sua** e algumas paredes/portões; camas de casas do mapa não contam. |
| Não consigo colocar um item | Quadrado vermelho: tem algo no lugar, está longe demais, é rua ou água. |
| Desempenho ruim no celular | Feche outras abas e apps; o jogo é leve, mas o mapa é grande. |

---

*Feito em HTML, CSS e JavaScript puros (Canvas 2D), sem bibliotecas externas. O co-op usa um servidor Node com WebSocket.*
