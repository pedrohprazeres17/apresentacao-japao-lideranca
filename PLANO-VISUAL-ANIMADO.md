# Plano visual — apresentação animada do Japão

## Objetivo

Transformar o conteúdo já aprovado em uma apresentação HTML de 13 telas com ritmo de palco, leitura rápida e identidade própria, preservando a fidelidade ao documento entregue.

## Público

Professora e turma da disciplina de Liderança. Exibição em projetor, com apresentação oral de quatro integrantes e duração estimada de 12–14 minutos.

## Direção visual

**Sumi editorial contemporâneo.** A linguagem combina papel quente, tinta preta, vermelho hinomaru, recortes de cartazes culturais e movimentos inspirados por pincel, shoji e impressão. O resultado deve parecer uma peça editorial sobre o Japão, não um template corporativo nem uma reprodução da SPARK.

## Tipografia e escala

- Títulos: `Bodoni 72` / `Didot` / `Iowan Old Style`, com contraste alto e escala entre 64 e 124 px.
- Texto funcional: `Avenir Next` / `Hiragino Sans` / `Arial`, entre 17 e 28 px.
- Microtexto: caixa alta, 11–14 px, espaçamento amplo.
- Numerais e palavras-chave grandes funcionam como elementos de composição.

## Paleta

- Papel: `#eee9de` — fundo principal.
- Tinta: `#11110f` — texto e telas dramáticas.
- Vermelho: `#c51f2b` — foco, Japão e progressão.
- Cinza mineral: `#8b877f` — apoio e legenda.
- Branco quente: `#faf7ef` — contraste.

## Componentes

- Marcador vertical de seção.
- Barra inferior de progresso com 13 pontos navegáveis.
- Contador de tela e rótulo da seção.
- Linhas editoriais, círculos solares e grades shoji.
- Linha do tempo, comparação, processo e sequência noturna com movimentos próprios.
- Visão geral navegável (`O`) e modo tela cheia (`F`).

## Blueprint

- Palco fixo de `1600 × 900`, escalado como uma peça única para preservar a composição em qualquer tela.
- Área útil 16:9, com margens generosas e composição assimétrica.
- Cada tela tem uma ideia principal e no máximo um bloco secundário.
- Alternância entre telas claras e escuras para marcar capítulos.
- Apenas uma cena permanece ativa; a transição cobre a cena anterior antes da troca e revela a seguinte depois.
- Não existem avanços automáticos: cada etapa responde ao clique, teclado ou gesto do apresentador.

## Sistema de movimento — versão 2

Cada mudança de tela tem uma transição própria, ligada ao tema da tela que entra. Todas são feitas com Web Animations API, sem blur e sem avanço automático.

| Entra | Transição | Ideia |
|---|---|---|
| 02 · O país | **Hinomaru** | O sol vermelho da capa cresce, cobre a tela e se abre em círculo ao redor do globo. |
| 03 · História | **Pincel sumi** | Três pinceladas de tinta cobrem a tela e depois são “apagadas”. |
| 04 · Cultura | **Shoji** | Duas portas de papel com treliça de madeira se fecham e se abrem. |
| 05 · Trabalho | **Katana** | Um corte diagonal parte a tela anterior em duas metades que caem. |
| 06 · Gestão | **Noren** | Cortinas de loja com o sol descem e se abrem como se alguém passasse por elas. |
| 07 · Contraste | **Painéis** | A metade escura (Japão) desce e a clara (Brasil) sobe, já formando a tela. |
| 08 · Sony | **Hanko** | Um carimbo vermelho “ソニー” bate na tela, explode em vermelho e encolhe até virar o sol do slide. |
| 09 · Sony no Brasil | **Mosaico** | Ladrilhos giram em onda diagonal. |
| 10 · Morita | **Obturador** | A tela fecha como uma câmera, dispara um flash e abre no retrato. |
| 11 · Uma noite | **Anoitecer** | Um pôr do sol desce e a noite toma a tela. |
| 12 · Fun fact | **Último trem** | Um trem iluminado atravessa a tela em alta velocidade. |
| 13 · Conclusão | **Amanhecer** | A luz sobe e o sol nasce no canto. |
| 01 · Capa (voltar) | **Cortina** | Cortina lateral simples. |

Dentro das telas:

- Títulos entram palavra a palavra, saindo de uma máscara; em “SONY” cada letra cai.
- Fotos e pinturas são reveladas por uma cortina e assentam com um leve zoom. Depois que tudo entra, nada fica se mexendo (movimentos contínuos causavam tremor na tela).
- No slide 3, a linha do tempo se desenha e a foto de 1945 “revela” como papel fotográfico.
- No slide 12, um relógio corre de 00:30 (último trem) até 05:00 (primeiro trem).
- O cursor some depois de 2,5 s parado.
- No slide 2, o primeiro comando revela o Japão no globo; o segundo avança.
- Com “reduzir movimento” ativo no sistema, tudo vira um corte rápido.
- Para testar uma transição específica: `index.html?slide=4&tr=katana`.

## Densidade

- Títulos curtos e dominantes.
- Texto de apoio reduzido ao necessário para sustentar a fala.
- Informações detalhadas permanecem no roteiro oral.
- O conteúdo aprovado não será ampliado com novos fatos nesta etapa.
