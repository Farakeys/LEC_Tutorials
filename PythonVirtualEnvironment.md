# Criando o ambiente Virtual e o Git

1. Criar pasta do projeto
2. Criar o ambiente virtual Python  
 Se o virtualenv não estiver instalado, use o comando  
 ```pip install virtualenv```  
 Após, é necessário ativar o ambiente virtual  
```virtualenv venv```
3. Criar dentro da pasta do projeto uma pasta *code*, que é a pasta que efetivamente será utilizada para a aplicação. É importante fazer isso para que o git não sincronize o ambiente virtual inteiro, somente o código:  
```mkdir code```
4. Criar o repositório *git* dentro da pasta *code*:  
```cd code```  
```git init```
Ou
5. Criar o repositório *git* dentro de sua pasta de projeto e criar um arquivo *.gitignore* onde serão especificados os arquivos e pastas que não serão sincronizados:
```git init```
O windows não apresenta suporte para criação de arquivos iniciando com '.' então nesse caso você precisará criar o arquivo com um nome qualquer (use o notepad, notepad++ ou VScode para isso) e renomeá-lo para *.gitignore* utilizando o Powershell, GitBash ou outro ambiente de terminal.  
*Sintaxe no Powershell:*  
```ren .\gitignore.txt .\.gitignore```  
*Sinaxe no GitBash:*  
```mv .\gitignore.txt .\.gitignore```  

# Para as tarefas do dia a dia
1. Inicializar o ambiente virtual  
```<caminho do arquivo>\venv\Scripts\activate  (para ativação via cmd do Windows)```  
2. Escrever o código desejado (arquivos, etc) na pasta code  
3. Para instalar uma extensão  
```pip install <extensão>``` (com ambiente virtual ativado)
4. Para adicionar ao Git Stack (use o parâmetro *--all* ou especifique os arquivos)  
```git add --all```   
5. Para fazer o commit  
```git commit -m "<identificação da versão>"```  
6. Para criar o arquivo de dependências  
```pip freeze > requirements.txt```
7. Para instalar um ambiente virtual novo a partir das dependências  
  Criar e ativar o virtual environment e depois utilizar o seguinte  comando do Python: ```pip install -r requirements.txt```
8. Para sair do ambiente virtual, utilizar o comando  
```deactivate```

# 
