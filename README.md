# Projeto: Infraestrutura AWS com Terraform – VPC + EC2

Este projeto é um laboratório prático de infraestrutura como código (IaC), com o objetivo de provisionar uma **VPC personalizada e uma instância EC2** na AWS utilizando Terraform.

---

## 🧱 Tecnologias Utilizadas

- **AWS** – Provedor de nuvem
- **Terraform** – Ferramenta de IaC
- **AWS CLI** – Interface de linha de comando para autenticação
- **Visual Studio Code** – Editor de código
- **Windows Terminal / PowerShell** – Terminal utilizado

---

## 🚀 O que será criado

- Uma **VPC personalizada**
- Subnet pública
- Internet Gateway
- Route Table
- Instância EC2 com:
  - Acesso SSH habilitado
  - Tag de identificação
- Segurança via **Security Group**

---

## 📁 Estrutura do projeto
infra-aws-vpc-ec2/ 
├── main.tf # Arquivo principal com os recursos 
├── variables.tf # Variáveis reutilizáveis
├── outputs.tf # Saídas úteis após o deploy

---

## ⚙️ Pré-requisitos

- Conta AWS com credenciais configuradas (via `aws configure`)
- Terraform instalado no seu sistema
- Permissões IAM para criação de recursos (EC2, VPC, etc)

---

## 📦 Como executar

```bash
# 1. Inicializar o Terraform
terraform init

# 2. Visualizar o que será criado
terraform plan

# 3. Aplicar a infraestrutura
terraform apply
