Universidade de Caxias do Sul - Centro de Computação e Tecnologia da Informação 

Disciplina: SIS0206A – Organização de Arquivos
Professor: Daniel Luis Notari
Especificação do Trabalho II - 2103-4
Este trabalho de implementação irá usar o arquivo de livros gerado para o trabalho I para as
tarefas 1 e 2. A tarefa 1 envolverá o uso de documentos XML, a tarefa 2 envolverá o uso de índices
em memória e a tarefa 3 envolverá o uso de bancos de dados NoSQL.
Tarefa 1 (Entrega em 11/11/2013)
Esta tarefa consiste em gerar um Documento XML com os nomes dos autores de livros e o
endereço lógico do registro do arquivo de dados de Livros usado no trabalho 1. O Documento XML
pode ser gerado conforme os modelos das Figuras 1 e 2. A diferença entre eles é que a Figura 1
mostra um documento XML com uma instância para cada autor organizada em níveis. A Figura 2
mostra o Documento XML construído com um elemento para cada autor onde as informações estão
colocadas como atributos.
<autores>
<autor>
<nome>coloque aqui o nome</nome>
<enderecos>
<endereco>coloque aqui o endereço do arquivo de dados</endereco>
<endereco>coloque aqui o endereço do arquivo de dados</endereco>
</enderecos>
</autor>
<autor>
<nome>coloque aqui o nome</nome>
<enderecos>
<endereco>coloque aqui o endereço do arquivo de dados</endereco>
<endereco>coloque aqui o endereço do arquivo de dados</endereco>
</enderecos>
</autor>
</autores>
Figura 1: Estrutura de níveis para o Documento XML de autores<autores>
<autor nome = “coloque aqui o nome” endereco = “endereços arquivo de dados</autor>
<autor nome = “coloque aqui o nome” endereco = “endereços arquivo de dados</autor>
<autor nome = “coloque aqui o nome” endereco = “endereços arquivo de dados</autor>
</autores>
Figura 2: Estrutura sem níveis para o Documento XML de autores
A segunda parte da primeira tarefa envolve a pesquisa neste documento XML. Para fazer a
pesquisa deve ser usado o caminhamento com as expressões XPATH (semelhantes ao
caminhamento de diretórios). Para tanto, use as API para Documentos XML DOM ou SAX para
fazer esta busca. Deve-se receber o nome do autor como entrada e, o programa deve devolver todos
os autores que satisfaçam a condição de pesquisa. Não é necessário mostrar os dados dos livros.
Para esta tarefa podem ser usadas coleções prontas das linguagens de programação.
Tarefa 2 (Entrega em 25/11/2013)
A tarefa 2 consiste em realizar a pesquisa por nome do autor usando uma estrutura de dados
em memória (lista encadeada ou árvore) como índice. Para tanto, deve-se ler o Documento XML
criado na tarefa 1 para a criação da estrutura de índice em memória. Deve-se implementar uma
consulta onde deve-se fornecer o nome do autor como dados entrada. Em seguida, o programa deve
pesquisar no índice todos os autores que satisfaçam a condição de pesquisa. O programa deve
acessar o arquivo de dados para buscar os dados dos livros. Estas informações devem ser mostradas
na tela. Lembre-se que por ser uma consulta por chave secundária, mais de uma informação pode
ser mostrada para o usuário. Para esta tarefa podem ser usadas coleções prontas das linguagens de
programação.
Tarefa 3 (Entrega em 11/12/2013)
Cada grupo deverá escolher uma ferramenta para trabalhar com dados não-estruturados (ou
NoSQL ou semelhante) dentre as ferramentas vistas em aula. O grupo deverá baixar a ferramenta,
instalá-la e criar um esquema para armazenar os dados do arquivo de livros criados no Trabalho I. O
grupo deverá apresentar mecanismos de consulta pelos campos do arquivo.Comentários gerais
O trabalho deve ser feito em grupos de quatro pessoas (nem mais nem menos). As
linguagens de programação C, C#, Phyton e Java podem ser usadas para o desenvolvimento deste
trabalho. O comando static não pode ser utilizado para as linguagens de programação orientadas a
objeto (e nem comandos semelhantes) na definição de atributos e métodos. Os programas fonte, o
arquivo de dados e os arquivos de índice devem ser salvos no webfolio da disciplina até a data
indicada no cronograma da disciplina. No dia da apresentação, cada grupo deverá demonstrar o
programa para o professor.
