---
sidebar_position: 1
---

# Project: Maju Mundur API

API for Maju Mundur Application

## Mohon diperhatikan

- tidak dapat delete produt yang sudah ter-relasi dengan transaction (error constraint)
- merchant dan customer dapat melakukan registrasi dengan fitur:
  - register customer
  - register merchant
- merchant dapat melakukan crud menggunakan fitur seluruh fitur dari product controller
- customer dapat melihat all product dan product by id dengan fitur:
  - get all product
  - get product by id
- setiap customer transaksi, customer mendapatkan point dengan nilai total price / 1000
- merchant dapat melihat history pembelian product dia, dengan menggunakan fitur:
  - get history merchant transaction, sesuai dengan user account id merchant yang login

## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  mvn install
```

**Configure your application properties**

Start the server

```bash
  mvn spring-boot:run
```

Start the swagger ui

```bash
  http://localhost:8080/swagger-ui.html
```

**Open with your idea or vscode**