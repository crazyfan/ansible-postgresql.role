```
Роль для развертывания Postgresql10
Для работы с postgresql использовать pgpool2 port 5433
Доступные параметры для применения: ./vars/main.yml
```
```
#### users, password, database
postgresql_user_name: test4
postgresql_user_password: testpass
postgresql_db_name: testpsdb4
postgresql_version: 10
#### postgresql
listen_addresses: "'localhost'"
listen_port: 5432
max_connections: 500
shared_buffers: 768MB
huge_pages: try
temp_buffers: 8MB
work_mem: 10MB
maintenance_work_mem: 64MB
autovacuum_work_mem: -1
dynamic_shared_memory_type: posix
effective_cache_size: 2GB
log_destination: "'stderr'"
datestyle: "'iso, dmy'"
timezone: "'W-SU'"
log_timezone: "'W-SU'"
default_text_search_config: "'pg_catalog.english'"
lc_messages: "'ru_RU.UTF-8'"                     
lc_monetary: "'ru_RU.UTF-8'"                     
lc_numeric: "'ru_RU.UTF-8'"   
lc_time: "'ru_RU.UTF-8'"
#### pgpool2
backend_hostname0: "'localhost'"
backend_port0: 5432
backend_weight0: 1
enable_pool_hba: off
num_init_children: 70
max_pool: 2
child_life_time: 300
child_max_connections: 0
connection_life_time: 0
client_idle_limit: 0
```
