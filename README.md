# GoTranslate 

O GoTranslate é um projeto feito dentro do google colab, desenvolvido durante a imersão IA da Alura.

### Qual a função do GoTranslate?

O GoTranslate é um sistema que busca ajudar o usuário a aprender inglês, focado na tradução de frases.

Ao utilizar o sistema o usuário tem acesso a um chatBot onde ele pode escolher um tema e um nível de dificuldade e a partir disso o bot cria frases em inglês para o usuário traduzir, a tradução é corrigida pelo bot que informa erros e acertos, além de dar dicas de como melhorar.

### Como usar?

Basta abrir o arquivo projeto imersão IA.ipynb no google colab e rodar tudo, na última célula de código irá rodar o chat

### Exemplo de uso:

- Tela inicial

![image](https://github.com/user-attachments/assets/79c1da5c-6968-4d82-95fe-7078901912af)

- Ao responder as perguntas iniciais

![image](https://github.com/user-attachments/assets/e1119b31-84a2-4556-ad29-c284051a7346)

- Pergunta e correção geradas:

![image](https://github.com/user-attachments/assets/04620044-a14d-4249-8570-4244a8e77c0d)


# Como funciona?

![image](https://github.com/user-attachments/assets/93f3221f-94a9-4e77-99d6-58855cfd0a02)

- Inicialmente o sistema funciona sem o uso de IA, perguntado o tema que o cliente deseja estudar e o seu nível de ingês
- Depois de receber essas informações o sistema utiliza os agentes para criar a frase
  - O primeiro agente busca frases possíveis sobre o tema escolhido pelo cliente
  - O segundo agente cria frases originais utilizando o retorno do primeiro agente
  - O terceiro agente isola uma frase e pede para o cliente traduzi-la
- Nesse momento o sistema espera o cliente traduzir a frase
- Depois é chamado o agente corretor que valida a tradução do usuário e da dicas de onde melhorar
- Por fim é perguntado se o cliente deseja continuar
- A resposta do cliente é tratada por um agente de continuidade para que o cliente não seja obrigado a enviar uma mensagem fixa e a comunicação fique mais natural
- Se o cliente desejar continuar o sistema volta para o primeiro agente, caso contrario se despede do usuario
