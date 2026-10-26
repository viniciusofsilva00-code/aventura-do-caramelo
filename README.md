# Aventura do Caramelo

Jogo de plataforma 2D no estilo 8-bit. Escolha um dos três cães e atravesse o quintal, o parque e os telhados da cidade até a casinha.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Modos

| Modo | Inimigos | Prêmio ao vencer o jogo |
|---|---|---|
| Fácil | cerca de metade | libera o Floquinho |
| Médio | quantidade normal | libera o Trovão |
| Difícil | quase o dobro | libera a Nevasca |

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

O primeiro pernil, que sai dos blocos, muda o cão para a segunda forma e aguenta um golpe extra. Pegar outro pernil nessa forma ativa o super poder por 15 segundos (a barra aparece embaixo do placar). Levar dano tira o pernil e o super poder.

## Regras

- Uma vida extra a cada 20 ossos (máximo de 9 vidas).
- Perdeu todas as vidas: a jornada recomeça na fase 1.
- Fases longas: quintal com 168 colunas (300 s), parque com 180 (400 s) e telhados com 192 (450 s).

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter ou Esc: pausar. No menu de pausa, escolha entre continuar e voltar ao menu inicial
- F: tela cheia · M: som
- No celular, botões na tela (TELA liga a tela cheia)

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>`, sem bibliotecas. A altura interna é de 240 pixels e a largura acompanha a janela (de 256 a 480). Sprites desenhados em código e sons gerados com Web Audio.

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, time, map}` ao array `LEVELS`. A legenda dos tiles está no topo do script.
