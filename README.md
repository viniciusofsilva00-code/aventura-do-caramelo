# Aventura do Caramelo

Jogo de plataforma 2D no estilo 8-bit. Na noite de São João, os fogos assustam os três cães da Vó Lurdes e cada um foge para um canto da cidade. Você escolhe um deles e atravessa o quintal, o parque e os telhados para reunir a matilha e voltar para casa.

## Personagens

| Cão | Raça | Velocidade | Pulo |
|---|---|---|---|
| Caramelo | vira-lata | média | médio |
| Paçoca | salsicha | alta | baixo |
| Pipoca | pug | baixa | alto |

Os amigos resgatados seguem você nas fases seguintes.

## Regras

- Vida extra aos 5.000, 12.000 e 20.000 pontos, e depois a cada 10.000 (também a cada 50 ossos). Máximo de 9 vidas.
- Perdeu todas as vidas: a jornada recomeça na fase 1.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter: iniciar e pausar · M: som
- No celular, botões na tela

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>` (256×240), sem bibliotecas. Sprites desenhados em código e sons gerados com Web Audio.

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, map}` ao array `LEVELS`. A legenda dos tiles está no topo do script.
