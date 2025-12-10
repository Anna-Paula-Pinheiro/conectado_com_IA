# 🤖 Conectado com IA: Primeiros Passos com a API do Gemini no Google Colab

Este repositório contém um notebook Google Colab que serve como um guia inicial e prático para interagir com o modelo de Inteligência Artificial **Gemini** utilizando a biblioteca oficial do Google para Python (`google-genai`).

O notebook demonstra como configurar o ambiente, realizar uma chamada simples para gerar conteúdo e, o mais importante, como estabelecer e manter uma conversa (chat) com o modelo.

## 🔗 Abrir no Google Colab

Você pode executar o código diretamente no seu navegador, sem necessidade de instalação local, clicando no botão abaixo:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anna-Paula-Pinheiro/conectado_com_IA/blob/main/Conectado_com_IA.ipynb)

---

## ✨ Funcionalidades Demonstradas

O notebook `Conectado_com_IA.ipynb` aborda os seguintes conceitos essenciais da API do Gemini:

1.  **Configuração de Ambiente:** Configuração segura da Chave de API através dos **Segredos do Google Colab**.
2.  **Geração de Conteúdo:** Uso do método `generate_content` com o modelo `gemini-2.5-flash` para obter respostas diretas a prompts.
3.  **Criação de Chat (Conversação Contextual):** Inicialização de um objeto de chat com `client.chats.create` para manter o histórico e o contexto da conversa.
4.  **Histórico do Chat:** Recuperação do histórico completo de mensagens com `chat.get_history()`.
5.  **Loop Interativo:** Implementação de um loop simples para que o usuário possa interagir continuamente com o modelo de chat.

---

## 🔑 Pré-requisitos e Configuração

Para executar este notebook, você precisará de uma Chave de API válida do Gemini.

### 1. Obter a Chave de API

Você pode obter uma chave de API gratuitamente no site oficial do Google AI Studio:
* [**Obtenha sua API Key aqui**](https://ai.google.dev/gemini-api/docs/api-key)

### 2. Configurar no Google Colab (MUITO IMPORTANTE!)

O notebook foi escrito para ler a chave de API de forma segura usando o recurso **Secrets (Segredos)** do Google Colab. Siga estes passos:

1.  Abra o notebook no Colab (clicando no link acima).
2.  Na barra lateral esquerda do Colab, clique no ícone de chave (🔒 **Segredos/Secrets**).
3.  Clique em **+ Adicionar novo segredo**.
4.  No campo **Nome**, digite exatamente: `GEMINI_API_KEY`
5.  No campo **Valor**, cole a chave de API que você obteve.
6.  Marque a opção **"Notebook access"** para permitir que o notebook use a chave.

Dessa forma, sua chave de API fica segura e não é exposta no código ou no repositório.

---

## 🏃 Como Executar

1.  Certifique-se de que sua `GEMINI_API_KEY` está configurada nos **Segredos** do Colab (ver seção acima).
2.  Execute todas as células do notebook em sequência (você pode usar o atalho `Ctrl+F9` ou o menu **Ambiente de execução > Executar tudo**).
3.  A última célula do notebook iniciará um **loop interativo** no qual você pode digitar perguntas.
4.  Para encerrar o chat interativo, digite a palavra `fim` quando solicitado a fazer uma pergunta.

### 💡 Exemplo de Interação:

Digite sua pergunta: O que é IA? Responda Sucintamente Inteligência Artificial (IA) é o campo da computação que permite a máquinas simular a inteligência humana para aprender, raciocinar, perceber e resolver problemas.

Digite sua pergunta: Quando foi lançado o chat GPT? O ChatGPT foi lançado em 30 de novembro de 2022.

Digite sua pergunta: fim
---

## 📚 Bibliotecas Utilizadas

* `google-genai`: A biblioteca oficial do Google para interagir com a família de modelos Gemini.
* `os`: Para manipulação de variáveis de ambiente.
* `google.colab`: Para acessar os segredos do Colab.

---

## 🧑‍💻 Contribuição

Sinta-se à vontade para fazer um fork deste repositório, propor melhorias ou abrir issues.

---
