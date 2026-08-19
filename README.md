# Portfólio Gamificado

Um portfólio interativo desenvolvido em formato de jogo de plataforma 2D. Este projeto demonstra habilidades práticas em Front-End e manipulação do DOM, substituindo a rolagem tradicional de uma página web por uma experiência dinâmica de exploração e gamificação.

## Como Funciona

A arquitetura do jogo foi construída de forma nativa com HTML, CSS e JavaScript Vanilla, dispensando bibliotecas externas ou a API `<canvas>`. 

* **Renderização:** Os elementos do cenário, plataformas e o próprio personagem são renderizados via manipulação direta do DOM, utilizando posicionamento absoluto e atualizações contínuas de coordenadas no CSS.
* **Física e Colisões:** A detecção de impacto foi implementada do zero utilizando o conceito de AABB (Axis-Aligned Bounding Box). O cálculo restringe a gravidade de forma precisa quando o *hitbox* do personagem sobrepõe as bordas superiores das plataformas.
* **Game Loop:** A fluidez da animação e o tempo de resposta aos comandos são sincronizados com a taxa de atualização do monitor através do método `requestAnimationFrame`.
* **Lógica de Gamificação:** O projeto inclui um quiz interativo que utiliza o algoritmo Fisher-Yates para embaralhar as perguntas. O usuário é recompensado ao provar conhecimentos teóricos, o que altera o estado do cenário (liberando áreas ocultas para parkour).

## Como Utilizar (Controles)

A navegação pelas minhas informações profissionais, projetos e habilidades exige interação ativa:

* **Setas (Esquerda / Direita):** Movimentação do personagem.
* **Barra de Espaço:** Pulo.
* **Tecla 'E':** Interação com os objetos do cenário (abre modais informativos, links para repositórios e inicia os desafios do Quiz).
