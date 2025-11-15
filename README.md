# LINUX COMMAND LINE

## Comandos básicos do linux/terminal

### Terminals e Shells

Exibe Hello, World! no terminal
```
echo 'Hello, World!'
```

"Quem sou eu?" exibe nome do usuário no terminal
```
whoami
```

Com sudo (super user do) exibe o usuário root
```
sudo whoami
```

REPL (Read, Eval, Print, Loop)
1. Lê o comando
2. Processa o comando e executa
3. Mostra o resultado na tela
4. Reinicia o processo

### Variáveis

Criar uma variável
```
variavel=valor ou variavel="valor"
```

Exibir o conteúdo
```
echo $variavel
```

Se o conteudo da variável for um comando, chamar a var irá executar o comando

### History

O comando history exibe o histórico dos últimos comandos digitados no sheel/terminal
```
history
```

Com o parâmetro -c, o histórico é limpado (mas ainda ficará no arquivo .bash_history, apenas é limpado da sessão atual do shell)
```
history -c
```
### Filesystem

No linux, tudo são arquivos, que ficam em diretórios, que são distribuidos no sistema como uma árvore (tree file system), sendo o ponto inicial a /

Print working directory (diretório atual)
```
pwd
```

Para listar o que tem no diretório atual
```
ls
```

E para listar o que tem em outro diretório
```
ls nome-diretorio/
```

Para mudar de um diretório ao outro
```
cd novo-diretorio ou cd ../ para voltar para o anterior
```

Caminhos relativos não começam com /, enquanto caminhos absolutos começam sempre com /
```
teste/downloads (relativo) /home/teste/downloads (absoluto) 
```

Comando cat (concatenate) exibe o conteúdo de um arquivo
```
cat README.md
```

Também concatena o conteúdo de vários arquivos
```
cat exemplo_renamed.txt novo_arquivo.txt
```

Exibir as primeiras n linhas do arquivo
```
head -n 10 exemplo.txt (exibe as primeiras 10)
```

Exibir as últimas n linhas do arquivo
```
tail -n 10 exemplo.txt (exibe as primeiras 10)
```

Comando less permite ver o conteúdo de um arquivo de forma páginada. As setas servem com navegação para cima e baixo, enter para pular para a próxima linha e espaço para uma página por vez.
```
less exemplo.txt
```

O comando touch atualiza a data e hora (metadados) de um arquivo. Por padrão, o arquivo não existir, touch irá criar esse arquivo e, por isso, é majoritariamente usado para criação de arquivos.
```
touch novo-arquivo.txt
```

Para criar um diretório (pasta) novo, use o comando mkdir (make directory)
```
mkdir novo_diretorio
```

Para mover um arquivo ou diretório de lugar, use o comando mv (move)
```
mkdir exemplo_arquivo.txt novo_diretorio (move o arquivo .txt para o novo_diretorio)
```

Para remover um arquivo, use rm (remove). Para remover recursivamente (o diretório e todo o conteúdo dentro dele) use rm -r
```
rm exemplo_arquivo.txt ou rm -r novo_diretorio
```

Para copiar um arquivo, use cp (copy). Para copiar um diretório e todo seu conteúdo, use cp -R (maíusculo)
```
cp exemplo_arquivo.txt destino/ ou cp -R diretorio_cheio destino/
```

Tilde, atalho para o seu diretório home
```
~ é igual a /home/seu-usuario
```

Grep, comando case-sensitive para pesquisar textos dentro de arquivos ou em resultados de outros comandos.
```
grep "hello" words.txt pesquisa a palavra hello dentro do arquivo words ou grep -r "hello" . ou diretorio/ para buscar recursivamente
```


