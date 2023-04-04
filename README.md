<h1> Desafio: Conhecendo o DynamoDB na prática</h1>

<p align="center"> 📜 <a href="https://academiapme-my.sharepoint.com/:p:/g/personal/camila_cavalcante_dio_me/EaXyYOjBaFpZjkxhexMo5EcBKMEEAI5t5aHlsTjnBQJlUw?e=nxdB6C"> README BASEADO NA APRESENTAÇÃO DO PROJETO</a> 📜 </P>
<p> Sejam bem-vindos ao desafio: <strong> Conhecendo o DynamoDB na prática.</strong><br>Desafio que tive a honra de co-criar com a plataforma de cursos online <strong><a href="https://web.digitalinnovation.one/">DIGITAL INNOVATION ONE PARA O BANCO PAN</a></strong> 💛🧡<br>
    💎 O objetivo principal é colocar em prática umas das ferramentas de persistência de dados da AWS: <strong>DYNAMODB</strong> através de um  desafio de projeto. </p>



<h2> 👣 Nosso Percurso</h2>

<p>
✅ Conhecer os conceitos básicos do DynamoBD<br>
✅ Criar uma tabela no DynamoDB utilizando o Amazon CLI<br>
✅   Inserir dados<br>
✅ Criar índices globais secundários<br>
✅ Realizar pesquisa<br>
✅ Compartilhar no GitHub<br>

</p>


<h2> 👣 Passo-a-Passo</h2>

<p>
<strong>	1.</strong> Vamos ABSTRAIR o DOMÍNIO Bootcamp e MODELAR seus ATRIBUTOS E MÉTODOS <br>
<strong>	2.</strong> Criaremos as CLASSES: Bootcamp, Cursos, Mentorias e Devs e vamos relaciona-las <br>
<strong>	3.</strong> As CLASSES Curso, Mentoria e Devs também serão MODELADOS, ou seja, criaremos seus ATRIBUTOS E MÉTODOS <br> 
<strong>	4.</strong> Para que o código fique mais legível e de fácil manutenção, iremos utilizar de algumas das ferramentas que o PARADIGMA DE ORIENTAÇÃO A OBJETOS (POO) nos oferece: ABSTRAÇÃO, ENCAPSULAMENTO, HERANÇA E POLIMORFISMO <br>
<strong>	5.</strong> E para representar CLASSES que foram criadas e relacionadas, iremos transforma-las em OBJETOS<br>
</p>

----

<h2> 📚 DYNAMODB </h2>

<p>
O Amazon DynamoDB é um serviço de banco de dados NoSQL totalmente gerenciado, com desempenho rápido e escalabilidade cuja disponibilidade alcança a porcentagem de 99.9%.
O DynamoDB:
🔸 Não é normalizado;
🔸 Não existe uma entidade por tabela
🔸 Sem joins para pesquisa de dados;
🔸 Mais indicado para arquiteturas de microsserviços;
🔸 As tabelas podem receber atributos de forma dinâmica
 <br>
Os pricipais componentes do DynamoDB são: 
</p>


<h3>🔺 TABELAS:</h3>

<p>
O dynamoDB armazena seus dados em tabelas. Tabelas são uma coleção de dados</p>

<h3>🔺 ITENS:</h3>

<p> Cada tabela pode conter zero ou mais itens. Um item é um grupo de atributos identificável exclusivamente entre todos os demais itens.</p>

<h3>🔺 ATRIBUTOS:</h3>

<p>Cada item é composto de um ou mais atributos. Um atributo é um elemento de dados fundamental, algo que não deve ser dividido.</p>

<h3> 🔺 CHAVE PRIMÁRIA:</h3>

<p>A chave primária identifica exclusivamente cada item na tabela de modo que não possa haver dois itens com a mesma chave.</p>

<h3> 🔺 PARTITION KEY:</h3>

<p>É uma chave primária simples. O valor da chave é a entrada para uma função hash. A saída dessa função hash determina onde o registro estará alocado fisicamente.</p>

<h3> 🔺 PARTITION KEY + SORT Key: </h3>

<p> É uma chave primária composta de dois atributos. A tabela pode conter uma partition key não única, mas a combinação das chaves deve ser única. Os atributos auxiliam na localização de um recurso e são considerados uma boa prática.</p>


<br>
<h2 align="center"> ‼️ OUTROS COMPONENTES DO DYNAMODB ‼️ </h2>
<p>
<h3>🔻 ITENS SECUNDÁRIOS:</h3> 
Permite consultar os dados na tabela usando uma chave alternativa, além de fazer consultas em relação à chave primária.

<h3>🔻 ÍNDICE SECUNDÁRIO GLOBAL: </h3> 
O DynamoDB é compatível com esse tipo de índice que possui uma chave de partição e uma chave de classificação que podem ser diferentes das contidas na tabela.

<h3>🔻 ÍNDICE SECUNDÁRIO LOCAL: </h3>
O DynamoDB é compatível com esse tipo de índice que possui a mesma chave de partição da tabela, mas uma chave de classificação diferente. A modelagem do DynamoDB é feita pensando em como consultar/pesquisar os dados após a implementação do banco. 

<h2 align=”center”> ✨ TIPOS DE DADOS </h2>
Podem ser :
🔸 Escalares: representam um valor exato, como número, boolean, string e nulo;
🔸 Documentos: representam uma estrutura complexa com atributos aninhados, com JSON;
🔸 Conjunto: representam um conjuntos de valores escalares, como conjuntos de strings, números e binários”.

<h2 align=”center”> ✨ MODOS DE LEITURA E GRAVAÇÃO </h2>
O modo de leitura e gravação impactam diretamente no custo financeiro da hospedagem do banco. Existem dois modos:
🔸 Sob Demanda: Opção de faturamento flexível, com capacidade de servir centenas de solicitações por segundo;
🔸 Provisionado: Especifica o número de leituras e gravações por segundo. Permite manter um controle sobre os custos.

------------
<br>

Este repositório foi criado para fins de estudo, então contribua com ele.<br>
Se te ajudei de alguma forma, ficarei feliz em saber. E caso você conheça alguém que se identifique com o conteúdo, não deixe de compatilhar.<br>
<br>
Se possível:<br>
⭐️  Star o projeto<br>
🐛 Encontrar e relatar issues<br>
</p>


------------

Disponibilizado com ♥ por [Danielle](https://www.linkedin.com/in/danielle1306/ "Danielle").


