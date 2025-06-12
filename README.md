# 🔺 UaiShop - Loja de Videogames

Este é um projeto de front-end que simula uma loja online de videogames, com um layout de página única (Single-Page Application). A interface é limpa, interativa e construída com tecnologias web fundamentais.

---

## ✨ Funcionalidades

-   **Visualização de Produtos:** Exibição dos produtos em uma grade clara e organizada.
-   **Carrinho de Compras Dinâmico:** Adicione itens ao carrinho e veja-o ser atualizado instantaneamente sem recarregar a página.
-   **Cálculo Automático de Total:** O valor total da compra é calculado em tempo real conforme os itens são adicionados.
-   **Navegação em Página Única:** Links de navegação que rolam suavemente para as seções correspondentes.
-   **Formulário de Contato:** Uma seção de contato com um formulário funcional (requer implementação de backend).

---

## 🚀 Tecnologias Utilizadas

-   **HTML5:** Para a estrutura e semântica do conteúdo.
-   **CSS3:** Para a estilização e o layout (via arquivo `style.css`).
-   **JavaScript (ES6+):** Para toda a interatividade, manipulação do DOM e lógica do carrinho de compras (via arquivo `script.js`).

---

## 📂 Estrutura do Projeto

O código está organizado da seguinte forma:

-   **`index.html` (ou `mk1.html`):** O arquivo principal que contém toda a estrutura da página.
    -   **`<header>`:** Cabeçalho com o nome da loja e a barra de navegação.
    -   **`<section id="home">`:** Banner de boas-vindas.
    -   **`<section id="products">`:** Seção onde os produtos são listados.
        -   Cada produto usa um atributo `data-price` para armazenar o preço, que é facilmente acessado pelo JavaScript.
        -   As imagens dos produtos estão embutidas em **Base64**, o que torna o arquivo HTML autossuficiente, sem a necessidade de arquivos de imagem externos.
    -   **`<section id="cart">`:** Seção dinâmica do carrinho, controlada inteiramente pelo JavaScript.
    -   **`<section id="contact">`:** Seção com o formulário de contato.

-   **`style.css`:** Contém todas as regras de estilo para tornar a página visualmente agradável.

-   **`script.js`:** O cérebro da aplicação.
    -   Incluso com o atributo `defer` para garantir que o HTML seja carregado antes da execução do script.
    -   Adiciona `EventListeners` aos botões "Adicionar ao Carrinho".
    -   Manipula o DOM para atualizar a lista de itens e o valor total no carrinho.

---

## 🏁 Como Executar

Este é um projeto de front-end puro, então não há necessidade de um servidor para a funcionalidade principal.

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/seu-usuario/UaiShop.git](https://github.com/seu-usuario/UaiShop.git)
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd UaiShop
    ```
3.  Abra o arquivo `index.html` (ou `mk1.html`) diretamente no seu navegador preferido (Google Chrome, Firefox, etc.).

E pronto! A loja estará funcionando.

---

## 🔮 Melhorias Futuras

-   [ ] Implementar o backend em **PHP** para que o formulário de contato envie e-mails de verdade.
-   [ ] Adicionar responsividade para uma melhor experiência em dispositivos móveis.
-   [ ] Criar uma página de "Finalizar Compra" mais detalhada.
-   [ ] Adicionar a funcionalidade de remover itens do carrinho.
-   [ ] Refatorar a listagem de produtos para carregá-los a partir de um arquivo JSON ou de uma API, em vez de estarem fixos no HTML.
