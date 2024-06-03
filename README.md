# Desafios de Código - Simulando Desafios com IAs Generativas
## 3 / 5 - Refatorando com Eficiência

# Desafio

Neste desafio, você será solicitado a fornecer uma breve descrição de boas práticas de refatoração de código em três áreas específicas: identificação clara de funções, separação da entrada de dados e uso de nomes descritivos para variáveis e funções. Cada descrição deve indicar como o código pode ser melhorado nesses aspectos. O objetivo é simularmos a ação de pesquisas em IAs Generativas de busca e pesquisa; dessa forma, cada entrada simula um bom prompt de pesquisa.

## Entrada

A entrada será uma string de texto que representa um bom prompt de pesquisa para IAs Generativas. Após inserir sua descrição, o programa irá processá-la e fornecer um retorno sobre a prática de refatoração sugerida. Se a entrada corresponder a uma das três áreas especificadas, o programa irá sugerir a respectiva melhoria. Caso contrário, informará que a opção é inválida.

## Saída

Após inserir sua descrição, o programa irá processá-la e fornecer um retorno sobre a prática de refatoração sugerida. Se a entrada corresponder a uma das três áreas especificadas, o programa irá sugerir a respectiva melhoria. Caso contrário, informe: Opção inválida.

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

| Entrada | Saída |
| --- | --- |
| Dica de boas práticas de refatoração de código, nas funções. | Separe funções em unidades coesas e com responsabilidades únicas. |
| Dica de boas práticas de refatoração de código, nas entrada de dados. | Valide e normalize as entradas para evitar inconsistências. |
| Dica de boas práticas de refatoração de código, nomenclaturas. | Use nomes descritivos para variáveis e funções. |

## Atenção

Se você não está familiarizado com a linguagem de programação, não se preocupe! Você pode usar uma das seguintes inteligências artificiais para te ajudar a entender o código:

- ChatGPT: [https://chat.openai.com/](https://chat.openai.com/)
- Copilot: [https://copilot.microsoft.com/](https://copilot.microsoft.com/)
- Gemini: [https://gemini.google.com/](https://gemini.google.com/)
- Amazon Q (Para Empresas): [https://aws.amazon.com/pt/q/](https://aws.amazon.com/pt/q/)

Abaixo adicionamos algumas sugestões de uso e prompts para te auxiliar na resolução:

| Sugestões de Uso | Sugestões de Prompts |
| --- | --- |
| Explicação de Conceitos | Pode me explicar o que são estruturas de dados e dar exemplos? |
| Entendimento do Problema | Quais são as restrições ou requisitos específicos que devo considerar neste desafio? |
| Sugestões de Abordagem | Quais são as etapas principais que devo seguir para resolver este desafio? |
| Ajuda na Depuração | Estou recebendo um erro de sintaxe neste trecho de código. O que pode estar errado? |
| Revisão de Algoritmos | Você pode revisar meu algoritmo de ordenação e me dar feedback sobre sua eficiência? |

# SOLUÇÃO COMENTADA:

    def identificar_funcoes(texto):
      # Retorna uma mensagem sobre separar funções em unidades coesas e com responsabilidades únicas.
      return "Separe funções em unidades coesas e com responsabilidades únicas."

    def entrada_de_dados(texto):
      # TODO: Retorne uma mensagem sobre validar e normalizar as entradas para evitar inconsistências.
      return "Valide e normalize as entradas para evitar inconsistências."

    def nomenclatura_significativa(texto):
      # TODO: Retorne uma mensagem sobre usar nomes descritivos para variáveis e funções.
      return "Use nomes descritivos para variáveis e funções."

    def processar_entrada(texto):
      # Dicionário mapeando textos para funções
      opcoes = {
          "Dica de boas práticas de refatoração de código, nas funções.": identificar_funcoes,
          "Dica de boas práticas de refatoração de código, nas entrada de dados.": entrada_de_dados,
          "Dica de boas práticas de refatoração de código, nomenclaturas.": nomenclatura_significativa
      }

    # Verifica se o texto está presente nas opções
    if texto in opcoes:
        # Chama a função correspondente ao texto e retorna o resultado
        return opcoes[texto](texto)
    else:
        # TODO: Retorne uma mensagem de opção inválida se o texto não estiver nas opções
        return "Opção inválida"

    def desafio():
      # Solicita uma entrada do usuário
      entrada = input()
      # Processa a entrada e obtém a saída
      saida = processar_entrada(entrada)
      # Exibe a saída
      print(saida)

    desafio()
