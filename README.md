# Playbook site.yml

Предназначен для Linux семейства CentOS, выполняет следующие задания: 
1. Скачивает rpm-пакеты Сlickhouse (пакеты перечислены в clickhouse_packages) версии, указанной в clickhouse_version (по умолчанию 22.3.3.44) и производит их установку. После установки Сlickhouse запускается как сервис. 
3. Скачивает архив Vector версии vector_version (по умолчанию 0.19.3) и распаковывает в директорию vector_dir (по умолчанию директория vector). Далее на основе шаблона vector.service формируется unit и запускается Vector в режиме сервиса.  

# Playbook site_alt.yml

Отличается от site.yml способом установки Vector (через rpm-пакет).   
