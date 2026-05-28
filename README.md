# Desafio das Letras 🧩🔤

O **Desafio das Letras** é um jogo de quebra-cabeça deslizante dinâmico e focado em palavras. O objetivo é mover as peças pelo tabuleiro aproveitando o espaço vazio para alinhar sequências de letras na horizontal ou na vertical e pontuar validando-as em tempo real.

O grande diferencial deste projeto é o foco em **acessibilidade digital (a11y)**, garantindo autonomia, navegação semântica fluida e usabilidade impecável para pessoas com deficiência visual usuárias de leitores de tela.

---

## 🕹️ Como Jogar

1. **O Tabuleiro:** É composto por uma matriz $4 \times 4$ contendo 15 letras sorteadas e 1 espaço vazio.
2. **Movimentação:** Você só pode mover letras que estejam diretamente adjacentes (em cima, embaixo, à esquerda ou à direita) ao espaço vazio. Ao ativar uma letra válida, ela desliza para o espaço livre.
3. **Objetivo:** Forme palavras de 3 ou mais letras nas linhas ou colunas do tabuleiro.
4. **Validação:** Clique ou ative o botão **"Validar Palavras"**. O jogo analisa o tabuleiro atual, consulta um dicionário via API e computa seus pontos.
5. **Dificuldade:** Se o tabuleiro estiver muito complexo ou sem opções de palavras, use o botão **"Resetar Tabuleiro"** para reembaralhar as letras.

---

## ♿ Recursos de Acessibilidade Implementados

Este projeto foi desenhado sob os padrões da **WCAG (Web Content Accessibility Guidelines)** e inclui:

* **Estrutura Semântica Baseada em Tabela:** O tabuleiro é renderizado utilizando tags HTML nativas (`<table>`, `<tr>`, `<td>`), permitindo que leitores de tela identifiquem perfeitamente as coordenadas espaciais das peças (linhas e colunas).
* **Gerenciamento de Foco Dinâmico:** Ao mover uma peça, o foco do teclado/leitor de tela acompanha o movimento e permanece na nova posição de forma inteligente, evitando que o usuário se perca na interface.
* **Textos Alternativos Dinâmicos (`aria-label`):** Cada botão do tabuleiro anuncia claramente a letra e a sua posição exata (Ex: *"Letra A. Posição linha 2, coluna 3"* ou *"Espaço vazio na linha 4, coluna 4"*).
* **Anúncios em Tempo Real (`aria-live`):** Feedbacks de erro, validação de palavras e pontuações são anunciados imediatamente pelo sintetizador de voz.
* **Sonoplastia Interativa (Web Audio API):** Feedbacks sonoros distintos sintetizados nativamente para cada ação: movimento bem-sucedido, movimento inválido, acerto de palavra e erro de validação.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estruturação semântica e acessível do DOM.
* **CSS3:** Estilização responsiva com variáveis nativas (`:root`), flexbox e transições sutis.
* **JavaScript (Vanilla JS):** Lógica do jogo baseada no algoritmo de embaralhamento *Fisher-Yates*, manipulação assíncrona (`async/await`) e gerenciamento de estados.
* **Web Audio API:** Geração de ondas senoidais e osciladores para os efeitos sonoros diretamente no navegador.
* **Dicio API:** Integração HTTP externa para consulta gramatical automatizada em português do Brasil.

---

## 🚀 Como Executar o Projeto

Como o jogo foi construído inteiramente em desenvolvimento frontend nativo, você não precisa instalar nenhuma dependência robusta:

1. Faça o download ou clone este repositório.
2. Abra o arquivo `index.html` diretamente em qualquer navegador moderno.
3. Certifique-se de interagir com a tela antes ou durante a inicialização para conceder permissão de áudio ao navegador.

---

## 👤 Autor

Desenvolvido com dedicação e foco em uma web mais inclusiva por **Anderson Carvalho**.
* **Contato:** [euconcego@gmail.com](mailto:euconcego@gmail.com)
