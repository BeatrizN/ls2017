# Lista 2 - Git (exercícios adicionais)

#### 1. Siga atentamente os slides disponíveis AQUI. Experimente os comandos, ambiente-se com eles. Esclareça suas dúvidas com o professor. Faça uso de repositórios locais e, para boa parte dos comandos, terá que interagir com o GitHub (serviço sugerido na disciplina). Faça isto antes de prosseguir com os demais itens.

#### 2. Qual o comando para que as “marcas” ou tags sejam enviadas para o repositório remoto? (um simples git push não produz este efeito)
<pre>git push --tags</pre>

#### 3. Qual o nome do branch padrão do Git?
<pre>Master</pre>

#### 4. O que o comando git branch <branchname> realiza?
<pre>Exibe os branchs do repositório com o nome fornecido.</pre>

#### 5. Como criar um branch a partir de um commit específico?
<pre>git branch <nome></pre>

#### 6. Em um repositório, qual o efeito do comando git branch erro1234?
<pre>Iria criar o branch erro1234</pre>

#### 7. Qual o comando para se alternar para um branch de nome experimento2?
<pre>Git branch <nome> <commit> </pre>

#### 8. Em um repositório com dois branches, b1 e b2, onde b1 é o corrente, qual o efeito do comando git branch?
<pre>Exibe b1.</pre>

#### 9. O que o comando git checkout -b novobranch faz?
<pre>Cria um novo branch chamado novobranch.</pre>

#### 10. Qual a função do comando git branch -d teste?
<pre>Remove o branch teste.</pre>

#### 11. Durante o desenvolvimento de um software é comum, por exemplo, utilizar um novo recurso por meio de experimentação. Talvez uma nova tecnologia, uma nova biblioteca que pode ser útil ao que está em desenvolvimento, ou até mesmo uma nova versão de um produto já empregado. Para que o uso deste novo recurso não interfira com o que é considerado pronto, um branch pode ser criado para a experimentação. Código que for criado para a experimentação existirá apenas nobranch criado. Se eventualmente o experimento demonstrar um resultado satisfatório, as alterações realizadas no branch poderão ser incorporadas no que é considerado pronto, ou seja, no branch principal (master). Esta última ação é conhecida por merge. Neste item, apresente uma sequência de comandos que simula um caso simples de criação e uso seguido de merge empregando um branch para ilustrar uma experimentação conforme acima. A sequência deve incluir, obrigatoriamente: (a) criação de um ou mais branches; (b) chaveamento para pelo menos dois branches e (c) merge. Para simular alteração em um arquivo, basta simplesmente fornecer algo como Arquivo <nome> é alterado. O que foi fornecido em negrito representa uma ação que altera um arquivo cujo nome é fornecido entre o sinal de menor e o de maior.  
<pre>git branch A</pre>
<pre>git checkout A</pre>
<pre>git checkout master</pre>
<pre>git merge A</pre>
<pre>git branch - d A</pre>
