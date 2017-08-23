# Lista 1 - Git (exercícios)

#### 1. Qual o comando para obter a versão instalada do Git?
git version

#### 2. Qual o efeito da execução de cada um dos comandos abaixo?
1. git config -l  
Ele lerá e escreverá a partir deste arquivo especificamente.
2. git mv a.txt b.txt  
Renomear arquivo
3. git reset –hard  
Retorna a copia de trabalho para o conteúdo do repositório (HEAD) Todo o conteúdo do repositório. Arquivos criados e não adicionados não são removidos.
4. git log -27  
Fornece muitos detalhes de cada commit
5. git help  
Disponibiliza ajuda das páginas de manual para qualquer comando do git.
6. git help reset  
Se obtem ajuda especifica especifica para o comando reset.
7. git add –all  
Prepara todos (--al) os seus arquivos para o commit.
8. git add -u  
Adiciona todos os arquivos todos os arquivos modificados que já são monitorados pelo git.

#### 3. O fluxo “clássico” de interação com o Git é algo como “realizar trabalho em um ou mais arquivos e diretórios”, “acrescentá-los para serem contemplados” e, finalmente, executar um “commit”. Quais os comandos necessários para realizar os dois últimos “passos” desse fluxo?
git add <nome>
git add -u
git commit -m “comentário”
git push

4. Qual o comando deve ser executado para identificar o que foi alterado desde o último “commit”?
gti show <commit>

5. Em um dado repositório, arquivos simplesmente copiados para lá, ou seja, untracked, podem ser exibidos/identificados com que comando?
git status
6. Qual o comando para efetuar um commit?
git push
7. Qual o comando que devemos empregar para descartar mudanças ocorridas no arquivo teste.txt, por exemplo?
git checkout teste.txt
8. O que deve ser feito para que um determinado diretório do seu repositório seja ignorado pelo Git?
git reset <nome>
9. O que acontece se o seu repositório local for removido?
A exclusão de um repositório privado irá apagar todos os seus garfos.
A exclusão de um repositório público não vai apagar os seus garfos.
10. Como clonar um repositório remoto?
git clone <URL>

11. Em alguns cenários git log pode produzir extensos resultados. Se houver interesse em visualizar o histórico de um repositório, onde cada mudança é fornecida exatamente em uma única linha, qual o comando que deve ser empregado?
git shortlog -sne

12. Em qual arquivo o Git armazena informações de configuração empregadas por usuário?
git config --global

13. Qual o comando para criar um repositório local?
git init

14. Qual o nome do diretório criado pelo Git quando se executa o comando git init?
origin

15. Qual o comando para adicionar todos os arquivos modificados? (Aqueles para os quais git status identificam como modified?)
git add -u
16. O Git faz uso do valor de hash conhecido por SHA1. O que isto significa? Qual o propósito? O que é SHA1?
É a chave de identificação de cada commit, usado para especifica-lo na hora de usar alguns comandos

17. Qual a palavra para indicar o último commit em vez do valor de hash SHA1 correspondente?
HEAD~1

18. Quando se cria dois arquivos usando um editor de texto qualquer e, na sequência, executamos o comando git add -u, os dois arquivos criados passam de untracked para new file?
Sim

19. Qual o efeito da execução dos dois comandos abaixo, nesta ordem, em um dado repositório?
git reset --soft HEAD~1 Se desfazer do último commit
git reset –hard Retorna a copia de trabalho para o conteúdo do repositório (HEAD). Exeto do ultimo commit por foi utilizado git reset --soft HEAD~1.

20. Após o emprego de um ambiente integrado de desenvolvimento (IDE), é comum a criação de arquivos e diretórios. Qual o comando que podemos empregar para remover arquivos e diretórios untracked?
git clean -f

21. Qual o nome do arquivo no qual podemos inserir a indicação para o Git de arquivos e diretórios a serem ignorados?
git checkout --<arquivo>

22. Quando se cria o arquivo MinhaClasse.class em um dado diretório e desejamos que o Git ignore não apenas este, mas arquivos .class em geral, por todos os membros de uma equipe que estão contribuindo com um dado projeto?
git reset HEAD

23. jQuery é uma famose biblioteca em JavaScript. Consulte detalhes em http://jquery.com. O repositório Git correspondente encontra-se disponível em https://github.com/jquery/jquery.git. Faça o clone deste repositório jqueryrepo.

24. No repositório jqueryrepo, criado no passo anterior, qual o efeito do comando 
git shortlog -sne?
Apresenta histórico do repositório, mas sem tantos detalhes como no git log

25. No repositório jqueryrepo, qual o efeito de git remote -v?
Exibe o nome e a URL do repositório.

26. Um repositório Git pode ser etiquetado ao longo do tempo. Ou seja, commits específicos podem ser “marcados” ou “etiquetados” para facilitar referências posteriores. Para listar todas as “etiquetas” (tags) estabelecidas para um dado repositório, qual comando deve ser executado?
git merge <branchNome>

27. Caso um dato repositório retorne muitas “marcas” ou “etiquetas” para o comando git tag, como retornar apenas aquelas que atendem a determinado padrão, por exemplo, iniciadas por 2.0?
git tag -a 2.0

28. Qual o efeito do comando git tag -a 3.4-gold -m “minha versão ouro”?

29. Após executado o comando acima, qual o efeito de git show 3.4-gold?
Exibe as diferenças introduzidas no repositório pelo ultimo commit.
30. O que o comando git push origin 3.4-gold teria como efeito?
Diria ao git para colocar os commit no repositório 3.4-gold

31. Após executar um commit, qual o efeito de git commit –amend?

32. Após executar git add x.txt, qual o efeito de git reset HEAD x.txt?
Ignora todos os arquivos .txt

33. Após alterar o conteúdo de um arquivo committed em passo anterior, qual o efeito do comando git checkout – a.txt?
Ignora a alteração do arquivo a.txt
34. Qual a diferença entre os comandos git reset HEAD x.txt e git checkout -- a.txt?
O comando git reset HEAD x.txt ignora o arquivo x.txt, já o comando git checkout – a.txt obtem a versão HEAD do arquivo no repositório em questão, esté é usado quando a alteração no arquivo foi equivocada e se deseja ignorá-la.
