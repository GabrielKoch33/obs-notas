services:
  redis:
    image: redis:latest
    container_name: redis_estudos
    ports:
      - "6379:6379"
    volumes:
      - redis_data:/data
    restart: unless-stopped
    command: redis-server --appendonly yes

volumes:
  redis_data:
--

services:
  mongo:
    image: mongo:latest
    container_name: mongo_estudos
    restart: unless-stopped

    environment:
      MONGO_INITDB_ROOT_USERNAME: admin
      MONGO_INITDB_ROOT_PASSWORD: admin123

    ports:
      - "27017:27017"

    volumes:
      - mongo_data:/data/db

volumes:
  mongo_data:

--


name: estudos_db

services:
  postgres:
    image: postgres:18
    container_name: db_postgres
    restart: always
    environment:
      POSTGRES_USER: postgres
      POSTGRES_PASSWORD: 250107gks
      POSTGRES_DB: postgres
    ports:
      - "5432:5432"
    volumes:
      - postgres_data:/var/lib/postgresql
    networks:
      - db_network
    healthcheck:
      test: ["CMD-SHELL", "pg_isready -U postgres"]
      interval: 5s
      timeout: 5s
      retries: 5

  pgadmin:
    image: dpage/pgadmin4
    container_name: db_pgadmin
    restart: always
    environment:
      PGADMIN_DEFAULT_EMAIL: gabrielkochsilva@gmail.com
      PGADMIN_DEFAULT_PASSWORD: 250107gks
    ports:
      - "5050:80"
    depends_on:
      postgres:
        condition: service_healthy
    volumes:
      - pgadmin_data:/var/lib/pgadmin
      - /home/gabriel/Documentos/repositorios_estudos/estudo_postgres:/var/lib/pgadmin/storage/gabrielkochsilva_gmail.com    
    networks:
      - db_network

networks:
  db_network:
    driver: bridge

volumes:
  postgres_data:
  pgadmin_data: