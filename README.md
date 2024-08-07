# Exercício 01

## Etapas do exercício de prática da Aula 02

### A - Criar o arquivo com conteúdo inicial
1. Comando:
   ```bash
   echo 01 > arquivo.txt
### B - Adicionar o arquivo no staging e conferir o status
1. Comando:
    ```bash
    git add arquivo.txt
    git status
 2. Saída de tela após adicionar o arquivo no staging:
 
    plaintext
    On branch main
    Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
    new file:   arquivo.txt
### C - Commitar o arquivo do staging
    Comando:
    ```bash
    git commit -m "git add example - arquivo.txt"

### D - Sobrescrever o conteúdo do arquivo.txt
    Comando:
    ```bash
    echo 02 > arquivo.txt
### E - Verificar o diffing no arquivo
    Comando:
    ```bash
    git diff arquivo.txt

### F - Adicionar novamente o arquivo no staging e conferir o status
    Comandos:
    ```bash
    git add arquivo.txt
    git status
    Saída de tela:
        On branch main
        Changes to be committed:
        (use "git restore --staged <file>..." to unstage)
        modified:   arquivo.txt
### G - Verificar o diffing no arquivo
    Comando:
    ```bash
    git diff --staged arquivo.txt
### H - Sobrescrever o conteúdo do arquivo.txt
    Comando:
    ```bash
    echo 03 > arquivo.txt

### I - Verificar o diffing no arquivo
    Comando:
    ```bash
    git diff arquivo.txt

### J - Fazer o restore do arquivo da área de staging e verificar o status
    Comandos:
    ```bash
    git restore --staged arquivo.txt
    git status

### K - Realizar o commit do arquivo e verificar o log
    Comandos:
    ```bash
    git commit -m "Atualiza arquivo.txt para 03"
    git log

### L - Adicionar um arquivo .gitignore com o seguinte conteúdo
    Comandos:
    ```bash
        echo "*.txt" > .gitignore
        git add .gitignore
        git commit -m "Adiciona .gitignore para ignorar arquivos .txt"
### M - Criar um arquivo novo.txt e verificar o status
    Comando:
        ```bash
        echo "conteúdo" > novo.txt
        git status
    Saída de tela:
        On branch main
        Untracked files:
    (use "git add <file>..." to include in what will be committed)
        novo.txt