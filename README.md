

# Cypress: app Web de Armazenamento de Imagens

Um aplicativo web simples e acessível para armazenar imagens no localStorage. Desenvolvido com as melhores práticas de acessibilidade.

## Funcionalidades

- **Armazenar Imagens:** Faça upload e salve imagens no localStorage do navegador.
- **Acessibilidade:** Totalmente acessível com navegação por teclado e suporte a leitores de tela.
- **Design Responsivo:** Funciona em dispositivos desktop e móveis.

## Como Começar

1. Clone o repositório:
    ```bash
    git clone https://github.com/erickwendel/vanilla-js-web-app-example.git
    ```
2. Navegue até o diretório do projeto:
    ```bash
    cd vanilla-js-web-app-example
    ```
3. Abra o arquivo `index.html` no seu navegador.

## Exemplo de Teste com Cypress

Você pode usar o Cypress para testes end-to-end. Aqui está um teste simples:

```javascript
describe('Armazenamento de Imagens', () => {
  it('Faz upload e exibe uma imagem', () => {
    cy.visit('/');
    cy.get('#uploadInput').attachFile('caminho/para/imagem.jpg');
    cy.get('#submitBtn').click();
    cy.get('#imageGallery').should('contain', 'imagem.jpg');
  });
});
```

## Demonstração ao Vivo

[Veja o app](https://erickwendel.github.io/vanilla-js-web-app-example/).

## Créditos

Este projeto foi baseado na vídeo aula disponível em [YouTube](https://youtu.be/56N0P67ffIA?si=WBfFYs8W4QgJE_CS).

![Captura de Tela do App](https://github.com/user-attachments/assets/a0f862f5-4e71-4933-bc10-cbb8c48ee046)
