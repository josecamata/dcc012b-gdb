# Depurando um código C/C++

## Atividades
### Usando VSCode + CMake-Tools
1. Verifique se a extensão CMake Tools está instalado no seu visual code. Instale se não estiver. 

2. Criando um CMakeLists.txt para compilar o código:
   - Tecle Ctrl + Shift + P para abrir a paleta de comandos  e digite *CMake Quick Start*
   - Indique o nome do projeto quando requisitado 
   - Selecione Kits disponivel. 

3. Modifique o arquivo CMakeLists.txt para compilar os arquivos testbed.c e matrix_multiply.c 

4. Observe na barra de comandos inferior que há atalhos para os comandos CMake.
   - Clique em CMake[Debug]: Ready para alterar o tipo de compilação.
   - Clique em [GCC xxxxx]: para alterar qual compilador será usado
   - Clique em Build para compilar o seu código
   - Em [all] você poderá ver quais executáveis estão disponíveis e selecionar um deles.
   - Selecione o seu executável (definido no CMakeLists.txt)
   - Clique no simbolo de play para executar
   - Clique na Joaninha para depurar

5. Observe a mensagem de erro, explore a interface de depuração do vscode.
  - Insere breakpoints no código e rode o codifo passo a passo.


### Usando terminal

Inicie uma sessão de depuração no GDB:

```
 $ gdb --args .build/executavel.exe
```
Este comando deve fornecer um prompt GDB, no qual você deve digitar run ou r:
```
 $ r
```
Seu programa irá travar, retornando um prompt, onde você pode digitar backtrace ou bt para obter um rastreamento de pilha (stack trace).







