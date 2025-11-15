# LINUX COMMAND LINE

## Comandos básicos do linux/terminal

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

## Variáveis

Criar uma variável
```
variavel=valor ou variavel="valor"
```

Exibir o conteúdo
```
echo $variavel
```

Se o conteudo da variável for um comando, chamar a var irá executar o comando

## History

O comando history exibe o histórico dos últimos comandos digitados no sheel/terminal
```
history
```

Com o parâmetro -c, o histórico é limpado (mas ainda ficará no arquivo .bash_history, apenas é limpado da sessão atual do shell)
```
history -c
```

