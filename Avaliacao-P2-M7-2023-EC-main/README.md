Criei 2 EC2, um para o back e outro para o front e baixei o repositorio do murilo
1 rds conectado com o EC2 do backend

para o back, eu modifiquei os dados do meu RDS.
Para o front eu alterei no arquivo script.js para o ip publico do Ec2 do backend na porta 8000 em todas as requisicoes 

No EC2 do front eu rodei isso

sudo apt update
sudo apt upgrade
sudo apt install apache2
# os arquivos do projeto devem estar em /var/www/html
git clone https://github.com/Murilo-ZC/Avaliacao-P2-M7-2023-EC.git
sudo cp ./Avaliacao-P2-M7-2023-EC/frontend /var/www/html



e no EC2 do back eu rodei isso

sudo apt update
sudo apt upgrade


git clone https://github.com/Murilo-ZC/Avaliacao-P2-M7-2023-EC.git

pip install -r requirements.txt

python main.py

Porem infelizmente eu nao consegui fazer o front fazer as requisicoes para o backend....

