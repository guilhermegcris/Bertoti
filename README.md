### Engenharia de Software
## Atividades 1 a 8

#1. Comentar com suas palavras o primeiro trecho do livro Software Engineering at Google, Oreilly:

O texto fala sobre as diferenças entre a engenharia de Software, Programação e Ciência da Computação, explicando principalmente que engenharia de software não se trata só de programar, já que esse segundo termo se refere mais especificamente a escrever código, enquanto o primeiro envolve aplicar conhecimento teórico e boas práticas para construir sistemas mais duradouros e confiáveis. Ele também faz uma comparação entre engenheiros de software com engenheiros de áreas tradicionais, que seguem regras e padrões rigorosos, e destaca que a área tecnológica possui mais falhas quanto à seguimento de processos e prosseguimento de métodos padrões. O texto também enfatiza que os softwares têm se tornado essenciais na sociedade, sendo cada vez mais importante adotar métodos mais rigorosos e profissionais, semelhantes aos de outras engenharias. O texto sugere no fim que o objetivo do livro é mostrar possibilidades para tornar o desenvolvimento de software mais confiável e estruturado, contribuindo para a evolução da profissão.

#2. Comentar com suas palavras o segundo trecho do livro Software Engineering at Google, Oreilly:

O texto explica fala novamente que a engenharia de software não é só escrever código, acrescentando que envolve todas as ferramentas, processos e práticas que podem ajudar uma empresa a criar e manter esse código ao longo do tempo. O foco é garantir que o software continue útil, sustentável e de qualidade, mesmo com as mudanças inevitáveis. Além disso, é destacado que a engenharia de software pode ser vista como “programação ao longo do tempo”. O texto também apresenta três princípios fundamentais que toda equipe de software deve considerar, que são tempo e mudança, escala e crescimento e custos e compensações. Por fim, é mostrado que a engenharia de software é sobre pensar no futuro, buscando práticas que tornem o código durável, escalável e sustentável.

#3. Listar e explicar 3 exemplos de tradeoffs:

Exemplo 1: Armazenamento local e Processamento em nuvem
É possível armazenar dados no dispositivo utilizado e será mais rápido e privado, porém exige mais recursos no processamento desses dados. Também é possível usar a nuvem para deixar o processamento mais leve, dependendo assim da internet.

Exemplo 2: Generalização e Simplicidade
É possível criar sistemas muito genéricos, mas pode haver maiores complicações no desenvolvimento do código de maneira desnecessaria, exigindo um grau de dificuldade maior do que o sistema que é feito para ser simples e resolver um problema pontual.

Exemplo 3: Custo e Escalabilidade
É possível criar um sistema capaz de suportar milhões de usuários, porém o nível exigido de infraestrutura e arquitetura serão amplamente mais custosos do que um sistema mais simples que suporta um número menos de pessoas

#4. Fazer 2 ou 3 exemplos de classes UML:
Exemplo 1:

      Aluno       

 - nome: String     
 - matricula: int   
 - nota1: double    
 - nota2: double    

 + calcularMedia(): double 
 + verificarAprovacao(): boolean


Exemplo 2: 

|        Produto         |

| - idProduto: int        |
| - nome: String          |
| - preco: double         |
| - estoque: int          |
--------------------------
| + atualizarEstoque(qtd: int): void |
| + calcularDesconto(porc: double): double |
| + exibirInfo(): void                |
--------------------------



#5. Fazer esses exemplos de UML em JAVA:
   
#6. Fazer testes customizados:
