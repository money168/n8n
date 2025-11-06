# n8n install local with docker compose
## n8n uses PostgreSQL database to save credentials, past executions, and workflows.

## env
The default database name, user and password for PostgreSQL can be changed in the .env file. 

## 

cat /etc/os-release  
sudo docker version  
sudo docker compose version  

mkdir n8n/n8n_data/ -p  
cd n8n  
sudo docker compose up -d  
sudo docker compose ps -a  

ss -ntlp  
ls -l n8n_data/  

docker compose pull n8n
docker compose up -d --no-deps n8n
