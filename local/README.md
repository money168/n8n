# n8n install local with docker compose

## n8n uses SQLite to save credentials, past executions, and workflows.

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
