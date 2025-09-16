# Industrial Investment Insights

This project analyzes industrial sector data to provide recommendations for better investment decisions.

**Stack:**
- Apache NiFi (Dockerized)
- PostgreSQL
- Power BI

**Deliverables:**
- Docker Compose for NiFi
- NiFi flow templates
- PostgreSQL schema & queries
- Power BI dashboard

**How to use:**

```sh
# Clone the repo
git clone https://github.com/husseinMohamed7/Industrial-Investment-Intelligence.git
cd Industrial-Investment-Intelligence
# Prepare Directories and Permissions (Linux)
sudo chown -R 1000:1000 ./nifi
sudo chmod -R 755 ./nifi
sudo chown -R 1000:1000 ./postgres
sudo chmod -R 755 ./postgres
# Start the Containers
docker-compose up -d
# get the username and password
docker logs nifi 2>&1 | grep -E "Generated (Username|Password)"
```
- Access NIFI in the browser:
    https://localhost:8443/nifi

- Access PostgreSQL in your favorite editor Port: 5432