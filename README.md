# robot
Robo em Python que vai interagir com o usuário
Claro! Aqui está um exemplo de código em Python de um robô que interage com o usuário:

```python
def saudacao_inicial():
    print("Olá! Eu sou um robô de interação.")
    print("Posso responder a algumas perguntas ou ter uma conversa simples.")
    print("Digite 'sair' a qualquer momento para encerrar nossa interação.")

def receber_mensagem():
    mensagem = input("Você: ")
    return mensagem

def enviar_resposta(resposta):
    print("Robô: ", resposta)

def processar_mensagem(mensagem):
    # Adicione lógica para processar a mensagem e gerar uma resposta adequada
    # Neste exemplo, a resposta é baseada em algumas regras pré-definidas
    if mensagem.lower() == "como você está?":
        return "Estou bem, obrigado por perguntar!"
    elif mensagem.lower() == "qual é o seu nome?":
        return "Meu nome é Robô 3000."
    elif mensagem.lower() == "qual é a sua função?":
        return "Minha função é interagir com os usuários e fornecer respostas."
    else:
        return "Desculpe, não entendi. Pode reformular sua pergunta?"

def main():
    saudacao_inicial()

    while True:
        mensagem = receber_mensagem()

        # Encerrar a interação se o usuário digitar "sair"
        if mensagem.lower() == "sair":
            print("Até logo!")
            break

        # Processar a mensagem e gerar uma resposta
        resposta = processar_mensagem(mensagem)

        # Exibir a resposta gerada
        enviar_resposta(resposta)

if __name__ == "__main__":
    main()
```
