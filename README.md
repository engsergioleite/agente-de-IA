# agente-de-IA
Pojeto agente de IA com RAG e LangGraph

Este projeto é a implementação de um agente de IA para triagem de solicitações, construído como parte da Imersão "Agentes de IA e Gemini" da Alura. O agente utiliza um modelo de linguagem do Google Gemini para interagir com o usuário, responder a perguntas com base em uma base de conhecimento (RAG) e automatizar fluxos de trabalho.

Contexto e Jornada de Aprendizado
Embora a imersão tenha sido construída para o Google Colab, este projeto foi desenvolvido no meu ambiente de trabalho padrão, o VS Code. Essa escolha me proporcionou um "curso extra" e me forçou a entender conceitos essenciais que um ambiente pré-configurado esconde.

Durante a construção, aprendi sobre:

Ambientes Virtuais (.venv): A importância de isolar as dependências do projeto para evitar conflitos.

Segurança e Publicação: Como proteger dados sensíveis, como a chave de API, usando um arquivo .env e garantindo que ele não seja publicado com o .gitignore.

Adaptações do Ambiente: As diferenças de execução entre o PowerShell e o CMD e a incompatibilidade de algumas bibliotecas (como IPython.display) com o VS Code.

OEssa escolha me fez aprender um curso extra de paciencia e utilizando a IA para me ajudar, me forçou a entender conceitos que um ambiente pré-configurado esconde. E foi aí que a minha jornada começou: Aprendi sobre ambientes virtuais (.venv), sobre como proteger minha api-key usando a pasta .env e adicionado ela no .gitignore para poder publicar o projeto no github com segurança, percebi algumas diferenças de execução entre o powershell e o cmd e algumas incompatibilidades como a biblioteca IPython.display que funciona no colab mas nao funcionou no VSCode.

Sobre o código da imersão, realmente teve muito Ctrl-C e Ctrl-V, considerei o código bem cheio de conceitos que não sabia e diante da dinamica da imersão, nada era tão detalhadamente explicado e sim bem corrido, o foco era fazer e não dar detalhes, até pela questão do tempo, dificultando a assimilação imediata de tantas bibliotecas, métodos e detalhes da própria linguagem python.

Consegui identificar e adaptar trechos de códigos que na dinamica do colab tinham ordens diferentes e ver alguns conceitos que já estudei em Python serem utilizados em um contexto de código muito maior que os usados nas aulas.

Funcionalidades do Projeto
O agente foi projetado para atuar como um triador de Service Desk, capaz de:

Tomar Decisões: Analisar a mensagem do usuário e decidir a melhor ação: AUTO_RESOLVER, PEDIR_INFO, ou ABRIR_CHAMADO.

Responder com RAG: Utilizar uma base de conhecimento (arquivos PDF) para responder a perguntas de forma automatizada e com citações.

Orquestrar Fluxos: Utilizar o LangGraph para criar uma lógica de fluxo de trabalho que guia a interação do agente.

