# Aventura do Caramelo

Jogo de plataforma 2D no estilo 8-bit. Escolha um dos três cães e atravesse o quintal, o parque e os telhados da cidade até a casinha.

**Jogar:** https://viniciusofsilva00-code.github.io/aventura-do-caramelo/

## Personagens

| Cão | Raça | Velocidade | Pulo | Com pernil |
|---|---|---|---|---|
| Caramelo | vira-lata | média | médio | capa de herói |
| Paçoca | salsicha | alta | baixo | piloto |
| Pipoca | pug | baixa | alto | realeza |

O pernil, que sai dos blocos, muda o cão para a segunda forma e aguenta um golpe extra.

## Regras

- Uma vida extra a cada 20 ossos (máximo de 9 vidas).
- Perdeu todas as vidas: a jornada recomeça na fase 1.
- Fases longas: quintal com 168 colunas (300 s), parque com 180 (400 s) e telhados com 192 (450 s).

## Controles

- Setas ou A/D: andar
- Espaço, W ou ↑: pular (segurar pula mais alto)
- Enter: iniciar e pausar
- F: tela cheia · M: som
- No celular, botões na tela (TELA liga a tela cheia)

## Como funciona

Um único `index.html` com HTML, CSS e JavaScript puro em `<canvas>`, sem bibliotecas. A altura interna é de 240 pixels e a largura acompanha a janela (de 256 a 480). Sprites desenhados em código e sons gerados com Web Audio.

Para adicionar uma fase, acrescente um objeto `{name, sub, theme, time, map}` ao array `LEVELS`. A legenda dos tiles está no topo do script.
