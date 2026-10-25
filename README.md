# Aventura do Caramelo

Jogo de plataforma 2D no estilo 8-bit: um vira-lata caramelo atravessa o quintal, o parque e os telhados da cidade até a casinha.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter: iniciar e pausar · M: som
- No celular, botões na tela

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>` (256×240), sem bibliotecas. Sprites desenhados em código e sons gerados com Web Audio.

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, map}` ao array `LEVELS`. A legenda dos tiles está no topo do script.
