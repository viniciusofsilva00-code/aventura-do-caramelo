# As Aventuras do Caramelo

Jogo de plataforma 2D no estilo 8-bit. Escolha um dos três cães e atravesse o quintal, o parque e os telhados da cidade até a casinha.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Modos

| Modo | Inimigos | Prêmio ao vencer o jogo |
|---|---|---|
| Fácil | cerca de metade | libera o Floquinho |
| Médio | quantidade normal | libera o Trovão |
| Difícil | quase o dobro | libera a Nevasca |
| Impossível | cerca de quatro vezes mais, e mais rápidos | libera o Parafuso |

Os cães liberados ficam salvos no navegador. Também existe um código secreto, digitado na tela inicial, que libera todos de uma vez.

## Personagens

| Cão | Raça | Velocidade | Pulo | 1 pernil | 2 pernis: super poder |
|---|---|---|---|---|---|
| Caramelo | vira-lata | média | médio | capa de herói | **Voo**: segurar o pulo no ar faz voar |
| Paçoca | salsicha | alta | baixo | piloto | **Turbo**: corre muito mais rápido e atropela os inimigos |
| Pipoca | pug | baixa | alto | realeza | **Terremoto**: pula mais alto e a aterrissagem derruba os inimigos por perto |
| Floquinho 🔒 | poodle | média | médio | bailarina | **Pulo triplo**: mais dois pulos no ar |
| Trovão 🔒 | pastor | alta | médio | policial | **Latido sônico**: ondas de latido derrubam os inimigos à frente |
| Nevasca 🔒 | husky | alta | alto | gelo | **Congelar**: os inimigos param e quebram ao encostar |
| Parafuso 🔒 | robô | média | médio | antena | **Ímã de ossos**: os ossos por perto vêm até ele |

### Parafuso, o cão-robô

- Sempre ativo: engole os gatos e não leva dano deles; os robôs aspiradores viram aliados, seguem ele e não machucam.
- Em compensação, com ele o mundo se desfaz:
  - um segundo depois do início, uma onda apaga o chão atrás dele. Ela fica mais rápida a cada fase e em modos mais difíceis, e acelera para alcançá-lo se ele abrir muita vantagem (perto de plataformas móveis ela desacelera um pouco);
  - pedaços de chão à frente tremem, racham e caem;
  - pedras caem do céu depois de um aviso vermelho e machucam o Parafuso.
- Depois da fase 3 vem o chefão **MECA-BIGODE**, um gato-robô gigante que corre, salta e atira parafusos. Ele machuca o Parafuso e precisa de 5 pisões na cabeça.

O primeiro pernil, que sai dos blocos, muda o cão para a segunda forma e aguenta um golpe extra. Pegar outro pernil nessa forma ativa o super poder por 15 segundos (a barra aparece embaixo do placar). Levar dano tira o pernil e o super poder.

## Regras

- Uma vida extra a cada 20 ossos (máximo de 9 vidas).
- Perdeu todas as vidas: a jornada recomeça na fase 1.
- Fases longas: quintal com 168 colunas (300 s), parque com 180 (400 s) e telhados com 192 (450 s).

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter ou Esc: pausar. No menu de pausa, escolha entre continuar e voltar ao menu inicial
- Esc ou Backspace: voltar (da escolha de modo para a de cão, e dela para a tela inicial); no celular, botão VOLTAR no canto
- F: tela cheia · M: liga e desliga som e música
- No celular: botão TELA CHEIA no menu e TELA durante o jogo. No iPhone (o Safari não permite tela cheia em páginas), use Compartilhar → Adicionar à Tela de Início e abra pelo ícone: o jogo roda sem a barra do navegador
- No celular, botões na tela (TELA liga a tela cheia)

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>`, sem bibliotecas. A altura interna é de 240 pixels e a largura acompanha a janela (de 256 a 480). Sprites desenhados em código; efeitos e músicas chiptune (menu, uma por fase, chefão e vitória) gerados com Web Audio a partir de partituras no próprio script (`SONGS`).

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, time, map}` ao array `LEVELS`. A legenda dos tiles está no topo do script.
