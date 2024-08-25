# Explorando os Recursos de IA Generativa com Copilot e OpenAI

![Static Badge](https://img.shields.io/badge/Status_Projeto:-Concluído(25/Ago/2024)-green)




![Static Badge](https://img.shields.io/badge/Inteligência_Artificial_(IA)-red)
![Static Badge](https://img.shields.io/badge/IA_Generativa-red)
![Static Badge](https://img.shields.io/badge/Transformers-red)
![Static Badge](https://img.shields.io/badge/Microsoft_Copilot-red)





## Introdução

Este repositório contém o material do laboratório 5 do Bootcamp da DIO, focado em explorar os recursos de IA generativa utilizando o GitHub Copilot e as ferramentas da OpenAI. O objetivo é proporcionar uma compreensão prática e aprofundada dessas tecnologias inovadoras.

## Objetivos

- **Entender o funcionamento do GitHub Copilot**: Como ele pode auxiliar na escrita de código de forma mais rápida e eficiente.
- **Explorar as ferramentas da OpenAI**: Utilização de modelos como GPT-3 e DALL-E para geração de texto e imagens.
- **Aplicação prática**: Desenvolver projetos que utilizem IA generativa para resolver problemas reais.

## Conteúdo

1. **Introdução ao GitHub Copilot**
   - O que é o Copilot?
   - Como configurar e utilizar no seu ambiente de desenvolvimento.
   - Exemplos práticos de uso.

2. **Explorando a OpenAI**
   - Introdução aos modelos GPT-3 e DALL-E.
   - Como utilizar a API da OpenAI.
   - Exemplos de geração de texto e imagens.

3. **Projetos Práticos**
   - Desenvolvimento de um chatbot utilizando GPT-3.
   - Criação de imagens com DALL-E.
   - Outros projetos sugeridos.

## Requisitos

- Conta no GitHub.
- Acesso ao GitHub Copilot.
- Chave de API da OpenAI.
- Conhecimentos básicos de programação.

## Como Usar

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/SimonePenido/DIO_Gen_IA_MS_Copilot.git


# DESENVOLVIMENTO:

## 1. Introdução ao GitHub Copilot

### O que é o Copilot?

O GitHub Copilot é uma ferramenta de inteligência artificial desenvolvida pela GitHub em parceria com a OpenAI. Ele atua como um assistente de codificação, sugerindo linhas de código e funções inteiras enquanto você programa. Utilizando modelos avançados de aprendizado de máquina, o Copilot é capaz de entender o contexto do código que você está escrevendo e fornecer sugestões relevantes.

### Como configurar e utilizar no seu ambiente de desenvolvimento

Para começar a usar o GitHub Copilot, siga os passos abaixo:

 **Instalação do Visual Studio Code**:
   - Baixe e instale o Visual Studio Code.

 **Instalação da extensão GitHub Copilot**:
   - Abra o Visual Studio Code.
   - Vá para a aba de extensões (ícone de quadrado no lado esquerdo).
   - Pesquise por "GitHub Copilot" e clique em "Instalar".

 **Login no GitHub**:
   - Após instalar a extensão, você será solicitado a fazer login na sua conta do GitHub.
   - Siga as instruções para autorizar o GitHub Copilot a acessar sua conta.

 **Configuração do Copilot**:
   - Após o login, o Copilot estará pronto para uso.
   - Você pode ajustar as configurações do Copilot acessando as preferências do Visual Studio Code.

### Exemplos práticos de uso

Aqui estão alguns exemplos de como o GitHub Copilot pode ser utilizado para melhorar sua produtividade:

1. **Completar funções automaticamente**:
   - Ao começar a digitar uma função, o Copilot pode sugerir a implementação completa com base no nome da função e nos parâmetros.

   ```python
   def calcular_area_do_circulo(raio):
       return 3.14159 * raio * raio

2. **Gerar código boilerplate**:
   - O Copilot pode ajudar a gerar código boilerplate, como a configuração inicial de um servidor web.
     

     ```JAVASCRIPT
     const express = require('express');
      const app = express();
      const port = 3000;

      app.get('/', (req, res) => {
      res.send('Hello World!');
      });

      app.listen(port, () => {
      console.log(`Servidor rodando em http://localhost:${port}`);
      });


  3. **Sugestões de código em tempo real**:
    - Enquanto você escreve, o Copilot oferece sugestões em tempo real que podem ser aceitas pressionando a tecla Tab.

         ```Java
           public class Main {
            public static void main(String[] args) {
            System.out.println("Hello, World!");
              }
         }


## 2. Explorando a OpenAI

### Introdução aos modelos GPT-3 e DALL-E

A OpenAI desenvolveu modelos de inteligência artificial avançados, como o GPT-3 e o DALL-E, que são capazes de gerar texto e imagens, respectivamente.

- **GPT-3 (Generative Pre-trained Transformer 3)**: É um modelo de linguagem que utiliza aprendizado profundo para produzir texto semelhante ao humano. Ele pode ser usado para uma variedade de tarefas, como tradução de idiomas, resumo de textos, geração de conteúdo e muito mais.
- **DALL-E**: É um modelo que gera imagens a partir de descrições textuais. Ele pode criar imagens realistas e artísticas baseadas em qualquer descrição fornecida.

### Como utilizar a API da OpenAI

Para utilizar a API da OpenAI, siga os passos abaixo:

1. **Crie uma conta na OpenAI**:
   - Acesse o site da OpenAI e crie uma conta.

2. **Obtenha uma chave de API**:
   - Após criar a conta, você poderá gerar uma chave de API que será usada para autenticar suas requisições.

3. **Instale a biblioteca OpenAI**:
   - Utilize o gerenciador de pacotes `pip` para instalar a biblioteca OpenAI em seu ambiente Python.
       ```bash
       pip install openai
   
4.**Configure a chave de API**:
    - Adicione sua chave de API no seu código para autenticar as requisições.
    
           ```Python

              import openai
      
                openai.api_key = 'sua-chave-de-api'



  5.**Configure a chave de API**:
  - Utilize a biblioteca para fazer uma requisição ao modelo GPT-3.

        ```Python

        response = openai.Completion.create(
        engine="text-davinci-003",
        prompt="Escreva uma história sobre um dragão e um cavaleiro.",
        max_tokens=100
        )

        print(response.choices[0].text.strip())


# Criação de imagens com DALL-E
Outro projeto interessante é a criação de imagens utilizando o modelo DALL-E. Você pode criar uma aplicação que gera imagens baseadas em descrições textuais fornecidas pelos usuários.

1. Configuração inicial:
Instale a biblioteca OpenAI.

    pip install openai


2. Código para gerar imagens:
Implemente um script que utiliza o DALL-E para gerar imagens.
Python

        import openai

        openai.api_key = 'sua-chave-de-api'

        prompt = "Um castelo medieval em um penhasco à beira-mar"
        response = openai.Image.create(
       prompt=prompt,
        n=1,
        size="1024x1024"
        )

        image_url = response['data'][0]['url']
        print(image_url)

  3. Crie uma interface simples para exibir as imagens geradas.
  Outros projetos sugeridos

  - Gerador de histórias: Utilize o GPT-3 para criar histórias baseadas em temas ou personagens fornecidos pelos usuários.
  - Assistente de programação: Desenvolva uma ferramenta que sugere trechos de código ou ajuda a resolver problemas de programação.
  - Aplicativo de arte generativa: Crie uma aplicação que gera arte abstrata ou paisagens baseadas em descrições textuais.
