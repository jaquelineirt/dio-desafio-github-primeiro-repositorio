# Desafio de Projeto sobre Git/GitHub da DIO
Repositório criado para o Desafio de Projeto.

## Anotações de Curso

1. Git é um sistema de versionamento de código distribuído;

2. Um sistema distribuído é um sistema que possui múltiplas cópias de si mesmo em diferentes locais;

3. Ambiente de desenvolvimento (local) é diferente do servidor (remoto);

4. Criar uma pasta que usarei para meus trabalhos;

5. Abrir o Git Bash nela;

   - **Cd** (e o nome da pasta criada) é o comando para selecioná-la no git bash;

   - **Ctrl + L** é o comando para limpar a tela;

   - Dentro da pasta você pode criar outra pasta usando o **mkdir**;

   - **dir** (Windows) e **ls** (Linux) retorna uma lista com o conteúdo contigo naquele diretório específico, você consulta o repositório;

   - **ls -a** mostra arquivos ocultos;

   - **Cd ..** volta um nível;

   - **git clone** faz um clone do repositório remoto em seu repositório local;

   - Um arquivo do tipo Markdown é um arquivo que uso caracteres especiais como # para formatar um texto.

### Estados

- Modificado (*modified*);
- Preparado (*staged/index*);
- Consolidado (*comitted*);

### Ajuda

Geral 

- git help

Comando específico

- git help add
- git help commit
- git help <qualquer_comendo_git>

### Configurações 

As configurações do Git são armazenadas no arquivo .gitconfig localizado dentro do diretório do usuário do Sistema Operacional (ex: Windows: C:/Users/Documents and Settings/user ou *nix/home/user).

As configurações realizadas através dos comandos abaixo serão incluídas no arquivo citado acima.

- Setar usuário (*git config --global user.name "Nome Usuário"*)
- Setar email (*git config --global user.email emailuser@mail.com*)
- Setar editor (*git config --global core.editor vim*)
- Setar ferramenta de merge (*git config --global merge.tool vimdiff*)
- Setar arquivos ignorados (*git config --global core.excludesfile ~/gitignore*)
- Listar configurações (*git config -list*)

##### Ignorar Arquivos

Os nomes de arquivos/diretórios ou extensões de arquivos listados no arquivo .gitignore não serão adicionados em um repositório. Existem dois arquivos .gitignore, são eles:

- **Geral**: Normalmente armazenado no diretório do usuário do Sistema Operacional. O arquivo que possui a lista dos arquivos/diretórios a serem ignorados por todos os repositórios deverá ser declarado conforme citado acima. O arquivo não precisa ter nome de .gitignore.
- **Por repositório**: Deve ser armazenado no diretório do repositório e deve conter a lista dos arquivos/diretórios que devem ser ignorados apenas para o repositório específico.

### Repositório Local

- **git init** inicializar o Git dentro de uma pasta em questão, cria novo repositório;
- **git status** verificar estado dos arquivos/diretórios;
- **git add meu_arquivo.txt** adicionar um arquivo em específico;
- **git add meu_diretorio** adicionar um diretório em específico;
- **git add .** adicionar todos os arquivos/diretórios;
- **git add -f arquivo_no_gitignore.txy** adicionar um arquivo que está listado no .gitignore;
- **git commit meu_arquivo.txt** comitar um arquivo;
- **git commit meu_arquivo.txt meu o_outro_arquivo.txt** comitar vários arquivos;
- **git commit meuarquivo.txt -m "new commit"** comitar informando mensagem;
- **git rm meu_arquivo.txt** remove arquivo;
- **git rm -r diretório** remove diretório;
- **git log** exibe histórico;
- **git log -star** exibe resumo do histórico;
- **git log --pretty=oneline** exibir informações resumidas em uma linha;
- **git log --pretty=format:"%h - %an, %ar : %s"**exibir histórico com formatação específica  - %h: Abreviação do hash; %an: Nome do autor; %ar: Data; %s: Comentário;
- **git log -- <caminho_do_arquivo>**exibir histório de um arquivo específico;
- **git log --summary -S<palavra_>[<caminho_do_arquivo>]**exibir histórico de um arquivo específico que contêm uma determinada palavra;
- **git log --diff-filter=M -- <caminho_do_arquivo>** exibir histórico modificação de um arquivo;
- **git log --author=usuário** exibir histórico de um determinado autor;
- **git blame -L 12,22 meu_arquivo.txt**exibir revisão e autor da última modificação de uma bloco de linhas;
- **git checkout -- meu_arquivo.txt**desfazendo alteração local;
- **git reset HEAD meu_arquivo.txt** desfazendo alteração local. Se o comando reset não alterar o diretório de trabalho, alteração pode ser realizada através do comando **git checkout meu_arquivo.txt**.

### Repositório Remoto

- **git remote ou git remote -v** exibir os repositórios remotos;
- **git remote add origin git@github.com:user/repositorio** vincular repositório local com um repositório remoto;
- **git remote show origin** exibir informações dos repositórios remotos;
- **git remote rename origin repositorio** renomear um repositório remoto;
- **git remote rm curso-git** desvincular um repositório remoto;
- **git push** enviar arquivos/diretórios para o repositório remoto
- **git pull** atualizar os arquivos no branch atual;
- **git fetch** buscar as alterações, mas não aplica-las no branch atual;
- **git clone git@github.com:user/repositorio** clonar um repositório remoto já existente.



## Links úteis
[Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/)

[Introdução ao Git e ao GitHub](https://docs.github.com/pt/get-started)
