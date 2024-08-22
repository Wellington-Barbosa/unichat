# Projeto UNICHAT

## Descrição

Este é um projeto de aplicação de chat multi-usuários desenvolvido em Python usando Flask e Flask-SocketIO. A aplicação foi criada para facilitar a comunicação entre colaboradores de um departamento, especialmente em um ambiente de HomeOffice. A aplicação permite que os usuários criem perfis simples, enviem mensagens em tempo real e compartilhem mídias como imagens e GIFs.

## Funcionalidades

- **Login Simples:** Os usuários podem inserir um nome para criar um perfil e iniciar a participação no chat.
- **Mensagens em Tempo Real:** As mensagens são enviadas e recebidas em tempo real utilizando Socket.IO.
- **Envio de Mídias:** Suporte para envio de imagens e GIFs, com redimensionamento automático para evitar poluição visual no chat.
- **Interface Responsiva:** A interface foi projetada para funcionar em diferentes tamanhos de tela, incluindo smartphones.
- **Tecla Enter para Enviar:** Os usuários podem enviar mensagens pressionando a tecla Enter.
- **Mídias em Buffer:** Ao selecionar uma mídia, ela é exibida na janela de mensagens antes de ser enviada definitivamente, permitindo que o usuário confirme a ação.
- **Design Personalizado:** Layout com ênfase na cor verde, um ícone visível no canto superior esquerdo, e uma menção ao desenvolvedor no rodapé ("By Wellington Barbosa").

## Particularidades

- **Não Armazenamento de Conversas:** As conversas não são armazenadas no servidor, garantindo privacidade.
- **VPN:** A aplicação está configurada para rodar em um ambiente local acessível por VPN, permitindo que colaboradores conectados à mesma rede VPN possam acessar o chat.
- **Problemas Conhecidos:**
  - Se muitas mensagens forem enviadas de uma vez, a rolagem automática pode parar de funcionar, necessitando um ajuste manual.
  - Em algumas telas de smartphones, pode haver desalinhamento ou sumiço de informações ao alternar entre o teclado e o campo de mensagens.

## Como Executar

### Pré-requisitos

- Python 3.7 ou superior
- Virtualenv instalado
- Acesso a uma VPN que permita tráfego entre clientes

### Passo a Passo

1. **Clone o Repositório:**

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio

2. **Crie e Ative o Ambiente Virtual:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
    
3. **Instale as Dependências:**
    ```bash
    pip install -r requirements.txt

4. **Execute a Aplicação:**
    ```bash
    python app.py

5. Acesse a Aplicação:

Acesse a aplicação em http://127.0.0.1:5000 ou, se estiver configurado, no IP atribuído pela REDE (http://IP_DA_REDE:5000).

## Notas de Implementação

* Firewall: Certifique-se de que a porta 5000 esteja aberta para conexões externas.
* Ambiente de Produção: Para ambientes de produção, considere usar um servidor web como Nginx e uma solução de WSGI como Gunicorn.

Desenvolvido como uma solução interna para facilitar a comunicação em um ambiente de trabalho distribuído.


### Explicações:

- **Seções:** O README contém seções padrão, incluindo descrição, funcionalidades, como executar e notas de implementação.
- **Detalhamento:** Foram incluídas instruções detalhadas sobre como configurar e executar a aplicação, assim como pontos importantes sobre sua implementação e uso.

Você pode personalizar esse arquivo conforme necessário para atender às especificidades do seu projeto. Se precisar de mais alguma modificação, estou à disposição!

By: Wellington Barbosa
