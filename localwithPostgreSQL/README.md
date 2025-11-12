# n8n install local with docker compose ( PostgreSQL)
n8n uses PostgreSQL database to save credentials, past executions, and workflows.  

### .env
The default database name, user and password for PostgreSQL can be changed in the .env file. 

### init.data.sh
https://github.com/n8n-io/n8n-hosting/blob/main/docker-compose/withPostgres/init-data.sh  

## start  
cat /etc/os-release  
sudo docker version  
sudo docker compose version  

mkdir n8n-postgres/n8n_data/ -p
cd n8n-postgres  
sudo docker compose up -d  
sudo docker compose ps -a  

ss -ntlp  
ls -l n8n_data/  

docker compose pull n8n
docker compose up -d --no-deps n8n


#### 20251112
