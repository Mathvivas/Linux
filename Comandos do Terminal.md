Ctrl + l ou clear 	--> Limpa o terminal

pwd 	--> Mostra o diretório atual


Clonar o repositório do Git: git clone [link do repositório (https://...)]


ls 	--> Mostra o conteúdo do diretório atual

README.MD --> Markdown

ls -a 	--> Mostra tudo

ls [diretório]  	--> Lista o conteúdo do diretório


cd [diretório] 	--> Entra no diretório  

cd .. 	--> Volta para o diretório pai

touch hello.py 	--> Cria o arquivo hello.py


mkdir Python 	--> Cria o diretório Python


mv hello.py Python/ 	--> Move o arquivo para o diretório


rm [arquivo] 	--> Remove o arquivo

rm -R [diretório]/ 	--> Remove o diretório


cat [arquivo] --> Lê o arquivo, mostra o que têm dentro


============================================================================================================


vi hello.py 	--> Cria o arquivo Python
Após entrar no editor vi, digitar 	--> :set number 	--> Numera as linhas
:wq 	--> Salvar e sair do vi


chmod +x hello.py 	--> Torna o arquivo executável


============================================================================================================


git status --> Verifica se existe algum arquivo que ainda não foi enviado para o Git

git add hello.py --> Adiciona o novo arquivo. Está pronto para ser empurrado para o Git

git commit -m "[comentário]" --> git commit -m "Criação do arquivo hello.py"

git push --> Envia os commits para o Git

git add ./ --> Add o diretório atual

Problemas --> git pull origin master

