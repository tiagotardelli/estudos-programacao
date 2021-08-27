## Principais Comandos

#### Atalhos

- Abrir o terminal.
  
  `Ctrl+Alt+T`

- Cancelar o comando atual, em primeiro plano ou segundo plano.
  `Ctrl+C`
- Pausar o comando atual, em primeiro plano ou segundo plano.
  `Ctrl+Z`
- Fazer o logout da sessão atual.
`Ctrl+D`
- Apagar a  última palavra.
`Ctrl+W`
- Apagar a linha inteira.
`Ctrl+U`
- Buscar um comando recente.
`Ctrl+R`
- Fazer logout da sessão atual
`exit`

#### Terminal
- Mostrar o caminho do diretório que você está 
`pwd`
- Listar as pastas e arquivos do diretório que você está
`ls`
- Listar as pastas e arquivos de um diretório
`ls <dretorio>`
- Listar com detalhes
`ls -l`
- Entrar no diretório
```shell
cd <dretorio>

cd Teste
```
- Voltar para o diretório anterior
`cd ..`
- Ir para o diretório principal do Linux 
`cd /`
- Voltar para o diretório home
`cd ~`
- taCriar um diritério
`mkdir`
- Remover um diretório ou arquivo
```shell
rm -r <diretorio>
rm <arquivo>

rm -r Teste
rm teste.txt
```
- Remover um diretório vazio
```shell
rmdir <diretorio>
  
rmdir Linux
```
- Obter ajuda sobre o comando
```shell
<comando> --help

ls --help
```
- - Abrir o manual do comando que deseja
```shell
man <comando>
```
- Trazer o histórico dos comandos executados no terminal
`history`
- Trazer o último comando digitado no terminal
`!!`
- Limpar o terminal
`clear`
- Renomear um arquivo/diretório
```shell
mv <diretorio_nome_atual> <diretorio_nome_novo>
mv <arquivo_nome_atual> <arquivo_nome_novo>

mv Teste linux
mv teste.txt linux.txt
```
- Mover um arquivo/diretório
```shell
mv <diretorio> <caminho>

mv Teste ~
```
- Criar arquivo vazio sem conteúdo
```shell
touch <nome_arquivo>

touch teste.txt
```
- Copiar um arquivo para um diretório
```shell
cp <nome_arquivo> <caminho>

cp linux.txt /home/usuario
```

- Exibir o calendário do mês corrente

```
cal
```

- Exibir a data atual

```shell
date
```

- Verificar o que determinado comando faz

  ```shell	
  whatis <comando>
  
  whatis cat ->> cat - concatenate files and print on the standard output
  ```

