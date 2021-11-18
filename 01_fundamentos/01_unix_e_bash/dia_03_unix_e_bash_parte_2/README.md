# Parte II - Manipulação & Busca
Neste exercício, exercitamos mais alguns comandos no terminal, como `wc`, `less` e etc.

Seguem os requisitos deste exercício e abaixo deles, a minha resolução. #VQV
#

1. Na pasta `unix_tests`, baixe um arquivo com os nomes de todos os países do mundo utilizando o comando `curl`:
```zsh
curl -o countries.txt "https://gist.githubusercontent.com/kalinchernev/486393efcca01623b18d/raw/daa24c9fea66afb7d68f8d69f0c4b8eeb9406e83/countries"
```

2. Mostre todo o conteúdo do arquivo `countries.txt` na tela.
```zsh
cat countries.txt
```

3. Mostre o conteúdo de `countries.txt`, página por página, até encontrar a `Zambia`.
```zsh
less countries.txt
```

4. Mostre novamente o conteúdo de `countries.txt` página por página, mas agora utilize um comando para buscar por `Zambia`.
```zsh
less countries.txt
/Zambia
```

5. Busque por `Brazil` no `countries.txt`.
```zsh
grep "Brazil" countries.txt
```

6. Busque novamente por `brazil`, mas agora utilizando o lower case.
```zsh
grep "brazil" countries.txt
```

Para os próximos exercícios, crie um novo arquivo chamado `phrases.txt` e adicione algumas frases à sua escolha. Não precisa criar o arquivo pelo terminal.
Criei um arquivo com as frases:
```
brown fox
strong lion
cute dog
```

7. Busque pelas frases que não contenham a palavra `fox`.
```zsh
grep -v "fox" phrases.txt
```

8. Conte o número de palavras do arquivo `phrases.txt`.
```zsh
wc -w phrases.txt
```

9. Conte o número de linhas do arquivo `phrases.txt`.
```zsh
wc -l phrases.txt
```

10. Crie os arquivos `empty.tbt` e `empty.pdf`.
```zsh
wc -l phrases.txt
```

11. Liste todos os arquivos do diretório `unix_tests`.
```zsh
ls
```

12. Liste todos os arquivos que terminem com `txt`.
```zsh
ls *.txt
```

13. Liste todos os arquivos que terminem com `tbt` ou `txt`.
```zsh
ls *.t{b,x}t
```

14. Acesse o manual do comando `ls`.
```zsh
man ls
```
