# skyChest

Backend desenvolvido com Java + Spring Boot focado em armazenamento/gerenciamento de pastas e arquivos na nuvem em sincronia com seu computador.

## Tecnologias

- Java 21
- Spring Boot
- Maven
- PostgreSQL
- Docker
- GitHub Actions
- GitHub Container Registry (GHCR)

---

## Funcionalidades

- API REST
- Integração com PostgreSQL
- Containerização com Docker
- CI automatizado com GitHub Actions
- Build e publicação automática de imagem Docker

---

# Como executar o projeto

## 1. Clonar repositório

```bash
git clone https://github.com/RafaelPastor/skyChest.git
```

---

## 2. Entrar na pasta

```bash
cd skyChest
```

---

## 3. Subir PostgreSQL com Docker

```bash
docker compose up postgres
```

---

## 4. Rodar aplicação localmente

```bash
./mvnw spring-boot:run
```

Aplicação disponível em:

```txt
http://localhost:8080
```

---

# Executando via Docker Image publicada

## 1. Baixar imagem

```bash
docker pull ghcr.io/rafaelpastor/skychest:latest
```

---

## 2. Rodar container

```bash
docker run -p 8080:8080 ghcr.io/rafaelpastor/skychest:latest
```

---

# Executando testes

```bash
./mvnw test
```

---

# CI/CD

O projeto possui pipeline automatizada com GitHub Actions:

- Build automático em Pull Requests
- Execução de testes automatizados
- Build de imagem Docker
- Publicação automática no GitHub Container Registry

---

# Docker Image

```bash
docker pull ghcr.io/rafaelpastor/skychest:latest
```
---

# Autor
Rafael Pastor