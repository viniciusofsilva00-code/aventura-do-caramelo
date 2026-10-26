# Aventura do Caramelo

Jogo de plataforma 2D no estilo 8-bit. Escolha um dos três cães da Vila Esperança e atravesse o quintal, o parque e os telhados da cidade, cada um com a sua própria história.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Personagens

| Cão | Raça | Velocidade | Pulo | Com pernil | Missão |
|---|---|---|---|---|---|
| Caramelo | vira-lata | média | médio | capa de herói | achar uma casinha para chamar de lar |
| Paçoca | salsicha | alta | baixo | piloto | recuperar a medalha roubada pelo gato Bigode |
| Pipoca | pug | baixa | alto | realeza | encontrar o lendário Pernil Dourado |

O pernil, que sai dos blocos, muda o cão para a segunda forma e aguenta um golpe extra.

## Regras

- Uma vida extra a cada 20 ossos (máximo de 9 vidas).
- Perdeu todas as vidas: a jornada recomeça na fase 1.
- A fase 3 é três vezes mais longa que as outras e tem 450 segundos.

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter: iniciar, avançar a história e pausar
- F: tela cheia · M: som
- No celular, botões na tela (TELA liga a tela cheia)

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>`, sem bibliotecas. A altura interna é de 240 pixels e a largura acompanha a janela (de 256 a 480). Sprites desenhados em código e sons gerados com Web Audio.

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, time, map}` ao array `LEVELS` e um capítulo em `STORIES` para cada cão. A legenda dos tiles está no topo do script.
