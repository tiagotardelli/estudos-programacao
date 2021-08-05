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



