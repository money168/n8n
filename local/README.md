# n8n install local with docker compose
n8n uses SQLite to save credentials, past executions, and workflows  

## start
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

## 注意事項
1.個人用於LAB.停用TLS/Https (N8N_SECURE_COOKIE=false)  
20251127  
1.add Environment variables
  - Reduce saved data  
  - Enable executions pruning，clear executions_data   
  - Clear SQLITE database  
