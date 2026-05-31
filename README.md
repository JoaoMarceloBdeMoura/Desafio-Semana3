# Desafio-Semana3
Desafio de python da semana 3 da trilha_python
semana3_desafio

Inventário de Reagentes de Laboratório

Explicação do funcionamento do programa

R: O programa simula um sistema de inventário de laboratório. Primeiro ele usa um set para descobrir quais são os reagentes únicos e quantos tipos diferentes existem. Depois ele usa zip para juntar as listas de reagentes, lotes e purezas em uma lista de tuplas. Em seguida, percorre essa lista usando unpacking para exibir um relatório dos frascos. Por último, utiliza List Comprehension para criar uma lista contendo apenas os lotes com pureza maior ou igual a 98%.

Como rodar o script

R: Basta executar o arquivo inventario_lab.py. O programa já possui os dados do inventário definidos nas listas e exibirá os resultados automaticamente.

Perguntas Teóricas

Levando em consideração a estrutura do nosso inventário, por que seria incorreto usar a função dict() para transformar o resultado do nosso zip() em um dicionário, utilizando o nome do reagente como "Chave" e o lote como "Valor"?

R: Porque existem vários reagentes repetidos. Como as chaves de um dicionário não podem se repetir, os valores antigos seriam sobrescritos e a gente perderia informações do inventário.

O que a função zip() gera na memória do Python antes de usarmos a função list() para forçar a visualização dos dados?

R: Ela gera um objeto do tipo zip, que é um iterável. Os dados só aparecem de forma visível quando percorremos esse objeto ou transformamos ele em uma lista.

Observando o seu código final, de que forma o List Comprehension substitui a necessidade de criar uma lista vazia e usar a estrutura de repetição for tradicional acompanhada do método .append()?

R: Com List Comprehension eu consigo criar e preencher a lista em uma única linha. Sem ela eu teria que criar uma lista vazia, fazer um for e usar append toda vez que encontrasse um lote aprovado.
