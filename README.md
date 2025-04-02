# notas-atletas
Olá pessoal!
Me chamo Felipe Pereira Gomes, tenho 32 anos, sou nascido e resido na cidade de Ponta Grossa/PR. Sou mestre e licenciado em Matemática pela Universidade Estadual de Ponta Grossa e estou iniciando minha jornada na carreira de programação. 
Aqui neste espaço quero demonstrar minha resolução para o primeiro desafio de certificação do curso da DEVstart, na trilha 1, Lógica de Programação. O título da tarefa é Pontuação dos atletas. Vamos lá!
O desafio consistia em calcular a média das notas de um conjunto de atletas, mas com uma particularidade: as notas a serem consideradas para o cálculo da média deveriam descartar a maior e a menor nota de cada atleta. Para resolver isso, desenvolvi uma função em JavaScript que percorre um array de objetos, onde cada objeto representa um atleta e suas respectivas notas.

A primeira etapa foi organizar os dados dos atletas em uma estrutura que facilitasse o cálculo. Para isso, utilizei um array de objetos, onde cada objeto contém:

nome: O nome do atleta.

notas: Um array de notas que o atleta obteve em suas competições.

Essa estrutura permitiu que o acesso às informações de cada atleta fosse simples e direto.

A função começou com a ordenação das notas de cada atleta em ordem crescente. Utilizei o método .sort() para garantir que as notas estivessem organizadas do menor para o maior valor. Isso é importante porque, ao calcular a média, precisávamos eliminar a maior e a menor nota, e a ordenação das notas simplifica essa tarefa.


Após a ordenação das notas, a próxima etapa foi eliminar a maior e a menor nota. Para isso, usamos o método .slice(1, -1) que seleciona um subconjunto do array, excluindo o primeiro (menor) e o último (maior) elemento. Isso resultou em um novo array de notas, o qual considerei para o cálculo da média.

Com as notas válidas (sem a maior e a menor), a próxima etapa foi calcular a média dessas notas. A função percorreu as notas restantes e somou os valores usando o método .forEach(). Depois de obter a soma das notas, dividimos pelo número de notas válidas (que é o comprimento do array de notas filtradas) para calcular a média.

Após o cálculo da média, a função exibiu os resultados no console. Para cada atleta, o nome, as notas originais e a média calculada foram exibidos. Utilizei o console.log() para garantir que os resultados fossem apresentados de forma clara e legível para o usuário.



