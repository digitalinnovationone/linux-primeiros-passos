# Mentoria Ao Vivo: Seus Primeiros Passos no Linux 🐧

## Descrição

Bem-vindo à Mentoria Ao Vivo "Seus Primeiros Passos no Linux". Esta sessão é uma introdução prática ao Linux, um sistema operacional de código aberto crucial em diversas áreas, incluindo cybersegurança, desenvolvimento de software, administração de sistemas, e muito mais. Nosso objetivo é fornecer uma base sólida para você se tornar um usuário proficiente do Linux. Esta mentoria é ideal para qualquer pessoa interessada em aprender os fundamentos do Linux. É particularmente útil para profissionais e entusiastas em áreas como cybersegurança, desenvolvimento, administração de sistemas, entre outras.

## Objetivos
- Compreender os conceitos fundamentais do Linux.
- Aprender e praticar comandos essenciais para a navegação e gerenciamento de arquivos.
- Familiarizar-se com o ambiente de terminal do Linux.

## Pré-requisitos
- Acesso a um terminal Linux 👩‍💻👨‍💻
   - Usando sua distro preferida, o WSL no Windows, ou uma opção online como o [https://copy.sh/v86](https://copy.sh/v86/).
- Curiosidade e vontade de aprender sobre o Linux.
  
## Dinâmica da Mentoria

### Preparação
- **Configuração Inicial:** Demonstração de como usar o [copy/v86](https://github.com/copy/v86) para acessar uma distribuição Linux.

### Exemplos Práticos

1. **Navegação Básica no Terminal**
   - `pwd` (para verificar o diretório atual)
   - `ls` (para listar conteúdos do diretório)
   - `cd nome_do_diretorio` (para mudar para outro diretório, use `..` para voltar)
   - **Exemplo Prático:** 
     - Criar um diretório: `mkdir dio`
     - Navegar para ele: `cd dio`
     - Verificar o diretório atual: `pwd`
     - Listar conteúdo (deve estar vazio): `ls`
     - Voltar para o diretório anterior: `cd ..`

2. **Manipulação de Arquivos e Diretórios**
   - `touch arquivo.txt` (para criar um novo arquivo)
   - `echo "texto aqui" > arquivo.txt` (adiciona um texto no arquivo, sobrescrevendo o conteúdo existente)
   - `echo "texto adicional" >> arquivo.txt` (adiciona um texto no fim do arquivo, mantendo o conteúdo existente)
   - `cp arquivo.txt destino/` (para copiar o arquivo)
   - `mv arquivo.txt destino/` (para mover o arquivo)
   - `rm arquivo.txt` (para remover o arquivo)
   - **Exemplo Prático:**
     - Criar arquivo: `touch mentoria.txt`
     - Incluir texto no arquivo: `echo "Seus Primeiros Passos no Linux" > mentoria.txt`
     - Adicionar mais texto no arquivo: `echo "Bem-vindo(a) à Mentoria!" >> mentoria.txt`
     - Copiar para 'dio': `cp mentoria.txt dio/`
     - Mover um arquivo: `mv mentoria.txt dio/mentoria_renomeado.txt`
     - Excluir arquivo: `rm dio/mentoria_renomeado.txt`

3. **Gerenciamento de Permissões em Arquivos**
   - `chmod 755 arquivo.txt` (para mudar permissões do arquivo)
   - **Exemplo Prático:**
     - Criar arquivo: `touch script.sh`
     - Criar arquivo: `echo "echo Hello Linux!" > script.sh`
     - Tenta executar o arquivo (deve dar erro): `./script.sh`
     - Mudar permissão: `chmod 755 script.sh`
     - Tenta executar o arquivo: `./script.sh`

   - **Tabela de Permissões Octal para `chmod`**

     | Número | Permissão    | Descrição                               |
     | ------ | ------------ | --------------------------------------- |
     | 7      | rwx (4+2+1)  | Leitura, escrita e execução             |
     | 6      | rw- (4+2)    | Leitura e escrita                       |
     | 5      | r-x (4+1)    | Leitura e execução                      |
     | **4**      | **r-- (4)**      | **Apenas leitura**                          |
     | 3      | -wx (2+1)    | Escrita e execução                      |
     | **2**      | **-w- (2)**      | **Apenas escrita**                          |
     | **1**      | **--x (1)**      | **Apenas execução**                         |
     | 0      | --- (0)      | Sem permissões                          |

   [Referência 'chmod'](https://guialinux.uniriotec.br/chmod/)

4. **Pesquisa de Arquivos**
   - `find . -name "*.txt"` (para encontrar arquivos .txt)
   - `grep "texto" arquivo.txt` (para buscar um texto específico dentro de um arquivo)
   - **Exemplo Prático:**
     - Buscar por arquivos .txt no diretório atual: `find . -name "*.txt"`
     - Buscar a palavra 'Linux' em todos os arquivos: `grep "Linux" *`

## Nota sobre Open Source e Licença GNU
- O Linux é um exemplo proeminente de um projeto open-source. Seu desenvolvimento é um esforço colaborativo de contribuidores ao redor do mundo, coordenado principalmente através do [repositório oficial do Linux no GitHub](https://github.com/torvalds/linux).
- O repositório desta mentoria segue a mesma licença GNU utilizada pelo Linux, refletindo nosso compromisso com a educação e a colaboração open-source.
