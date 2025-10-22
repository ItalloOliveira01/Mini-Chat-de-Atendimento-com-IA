# Chatbot Simples em JavaScript

Este projeto é um **chatbot simples** implementado em JavaScript que responde perguntas do usuário com base em palavras-chave. É uma aplicação básica para demonstrar interação entre o usuário e um assistente virtual em uma página web.

## Funcionalidades

* Recebe perguntas digitadas pelo usuário.
* Responde automaticamente com base em palavras-chave (`horário`, `preço`, `curso`).
* Resposta padrão caso a pergunta não seja reconhecida.
* Adiciona perguntas e respostas à tela em tempo real.
* Limpa o campo de input após o envio.
* Rolagem automática para sempre mostrar a última mensagem.
* Suporte para envio de mensagens ao pressionar a tecla **Enter**.

## Como usar

1. Crie um arquivo HTML com os seguintes elementos:

```html
<input type="text" id="pergunta" placeholder="Digite sua pergunta...">
<div id="mensagens"></div>
```

2. Inclua o arquivo JavaScript ou o script diretamente na página:

```html
<script src="chatbot.js"></script>
```

3. Abra a página no navegador e digite perguntas no campo de input. O assistente responderá automaticamente.

## Exemplo de Perguntas e Respostas

| Pergunta do usuário          | Resposta do assistente                                              |
| ---------------------------- | ------------------------------------------------------------------- |
| Qual é o horário?            | Nosso horário de atendimento é das 8h às 18h.                       |
| Qual o preço?                | Os preços variam conforme o serviço. Deseja falar com um atendente? |
| Quais cursos vocês oferecem? | Temos cursos de HTML, CSS e JavaScript disponíveis!                 |
| Pergunta desconhecida        | Desculpe, não entendi.                                              |

## Estrutura do Código

* **Função `responder()`**:

  * Obtém o texto do input do usuário.
  * Adiciona a pergunta à tela.
  * Verifica palavras-chave e define a resposta.
  * Adiciona a resposta à tela.
  * Limpa o input e faz a rolagem automática.

* **Event Listener no input**:

  * Detecta quando a tecla Enter é pressionada.
  * Chama a função `responder()` sem quebrar a linha no input.

## Tecnologias Utilizadas

* HTML para estrutura da página.
* CSS para estilização da página.
* JavaScript puro para manipulação do DOM e lógica do chatbot.

## Próximos Passos / Melhorias

* Implementar um sistema mais avançado de detecção de intenção.
* Adicionar respostas dinâmicas ou integração com APIs externas.
* Melhorar o estilo do chat com CSS.

