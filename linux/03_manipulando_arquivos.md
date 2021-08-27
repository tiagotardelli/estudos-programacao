## Manipulando de Arquivos

- Editor de texto nano

```shell
nano <nome_arquivo>

nano teste.txt
```

- Visualizar o conteúdo de um arquivo

``` shell
cat <nome_arquivo>

cat teste.txt
```

- Inverter as linhas do arquivo e exibir

```
tac <nome_arquivo>

tac teste.txt
```

- Imprimir as 10 primeiras linhas de um arquivo

```shell
head <nome_arquivo>

head teste.txt
```

- Imprimir as 10 últimas linhas do arquivo

```
tail <nome_arquivo>

tail teste.txt
```

- Enviar informações de um arquivo para outro

```shell
<comando> > <arquivo_novo>
<comando> + <arquivo> > <arquivo_novo>

cal > calendario.txt
cal 2020 > calendario.txt
cal jan 2020
tail testes.txt > novo.txt
head testes.txt > novo2.txt
```

- Adicionar informações em um arquivo

```shell
<comando> >> <nome_arquivo>

date >> calendatio_aug.txt
```

- Executar mais de um comando

```
<comando_1> | <comando_2> | <comando_n>

tail distros.txt | grep Linux
```

- Procurar uma palavra em um arquivo

```
grep <palavra>

tail distros.txt | grep Linux
```

- Paginar um arquivo para leitura

```
cat <nome_arquivo> | more
cat <nome_arquivo> | less

cat teste.txt | more
cat teste.txt | less
```

- Executar dois comandos consecutivos

  ```shell
  cat <nome_arquivo> & cat <nome_arquivo> -- saída aguardando enter
  cat <nome_arquivo> && cat <nome_arquivo> -- uma saída só
  
  cat teste.txt & cat teste2.txt
  cat teste.txt && cat teste2.txt
  
  mkdir linux && cd linux -- cria a pasta e já entra nela
  ```

- Usar o comando file para saber o tipo do arquivo

  ```shell	
  file <nome_arquivo/diretorio>
  
  file arquivo.txt ->> UTF-8 Unicode text
  file diretorio_atula ->> directory
  ```

- Procurar um arquivo pelo nome

  ```shell	
  find ~ -name <nome_arquivo>
  
  find ~ -name  distros.txt ->> mostra o caminho do arquivo 
  ```

  

| COMANDO | DESCRIÇÃO DO COMANDO                            |
| ------- | ----------------------------------------------- |
| cat     | Exibe conteúdos de arquivo no terminal          |
| tac     | Exibe a ordem inversa dos conteúdos no terminal |
| nano    | Editor de textos linux                          |
| touch   | Criar arquivos vazios                           |
| find    | Buscar arquivos                                 |
| file    | Exibe o tipo de um arquivo                      |
| head    | Exibe as 10 primeiras linhas de um arquivo      |
| tail    | Exibe as 10 últimas linhas de um arquivo        |
| more    | Exibe a paginação em um arquivo de texto        |
| less    | Exibe paginação em um arquivo de texto          |
| grep    | Busca palavras em arquivos texto                |
| cal     | Exibe calendário                                |
| date    | Exibe a data atual                              |
| whatis  | Exibe uma explicação sobre o comando            |

| OPERADOR | DESCRIÇÃO DO OPERADOR                                        |
| :------: | ------------------------------------------------------------ |
|    \|    | Envia a saída de um comando para entrada de outro comando permitindo a execução de dois comandos. |
|    >     | Redireciona a saída de um comando para outro comando arquivo. |
|    >>    | Redireciona a saída e adiciona a mesma para um comando ou arquivo. |
|    <     | Direciona a entrada de um arquivo para a saída de um comando. |
|    &     | Este operador permite usar dois comandos e separar suas saídas no terminal |
|    &&    | Usado para que dois comandos só sejam executados se o primeiro for executado com sucesso. |

