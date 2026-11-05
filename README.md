# 🚀 DevOps Lab — Infrastructure as Code & Automation

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-blue)
![Terraform](https://img.shields.io/badge/Terraform-IaC-7B42BC?logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-Automation-EE0000?logo=ansible&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containers-2496ED?logo=docker&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-Observability-425CC7?logo=opentelemetry&logoColor=white)

> Um laboratório prático de infraestrutura, automação, integração contínua e observabilidade, construído para transformar conhecimento em experiência real.

## 🎯 Sobre o projeto

O **DevOps Lab** é um projeto de aprendizado baseado em desafios práticos, desenvolvido ao longo de um bootcamp intensivo de **10 dias e 60 horas**.

O objetivo é integrar tecnologias utilizadas em ambientes corporativos para construir uma infraestrutura automatizada, reproduzível, versionada e monitorada.

Mais do que aprender ferramentas isoladamente, o foco é compreender como elas trabalham juntas no ciclo de vida de uma aplicação.

## 🧰 Stack tecnológica

| Tecnologia | Responsabilidade |
|---|---|
| **Hyper-V** | Plataforma de virtualização |
| **Ubuntu Server 26.04 LTS** | Sistemas Linux do laboratório |
| **Terraform** | Provisionamento de infraestrutura como código |
| **Ansible** | Gerenciamento de configurações e automação |
| **GitHub Actions** | Integração e entrega contínua |
| **Docker** | Containerização de aplicações |
| **OpenTelemetry** | Instrumentação e coleta de telemetria |
| **Grafana LGTM** | Observabilidade de aplicações |
| **Git & GitHub** | Versionamento e colaboração |

## 🏗️ Arquitetura proposta

```text
                   GitHub Repository
                          |
             +------------+------------+
             |                         |
         Terraform                GitHub Actions
             |                         |
             v                         |
        Hyper-V Host                   |
             |                         |
             v                         |
       Ubuntu Server VM <--------------+
             ^
             |
          Ansible
       Configuration
             |
             v
       Docker Runtime
             |
             v
       Application API
             |
             v
        OpenTelemetry
             |
             v
        Grafana LGTM
```

**Fluxo esperado:**

1. Terraform provisiona a infraestrutura no Hyper-V.
2. Ansible prepara o sistema operacional e instala os serviços.
3. GitHub Actions executa testes, build e deploy.
4. Docker hospeda a aplicação.
5. OpenTelemetry e Grafana fornecem visibilidade sobre desempenho, erros e comportamento da aplicação.

## 📚 Roadmap de aprendizado

- [x] **Dia 01:** Preparação do laboratório, Ubuntu Controller, rede e Ansible
- [ ] **Dia 02:** Ansible — inventários, módulos e primeiros playbooks
- [ ] **Dia 03:** Ansible — roles, Docker e automação Windows
- [ ] **Dia 04:** Terraform — fundamentos de infraestrutura como código
- [ ] **Dia 05:** Terraform — provisionamento no Hyper-V
- [ ] **Dia 06:** GitHub Actions — fundamentos de CI/CD
- [ ] **Dia 07:** CI/CD — build e deploy automatizado com Ansible
- [ ] **Dia 08:** APM — OpenTelemetry e fundamentos de observabilidade
- [ ] **Dia 09:** APM — Grafana, traces, métricas e alertas
- [ ] **Dia 10:** Projeto integrador — automação de ponta a ponta

## 📂 Estrutura do repositório

```text
devops-lab/
├── .github/
│   └── workflows/
├── terraform/
│   └── hyperv/
├── ansible/
│   ├── inventory/
│   ├── playbooks/
│   └── roles/
├── app/
├── observability/
├── docs/
└── README.md
```

## 🔬 Ambiente de laboratório

O projeto utiliza um host **Microsoft Hyper-V com Windows Server 2022**, executando máquinas virtuais Linux em uma rede interna dedicada.

O Ansible Controller utiliza Ubuntu Server 26.04 LTS e servirá como ponto central de gerenciamento das configurações.

O ambiente é isolado dos recursos de produção para permitir experimentação, testes e evolução contínua.

## 🔮 Próximas evoluções

Após a conclusão do projeto principal, estão previstas novas automações:

- Integração automática de servidores Ubuntu ao Active Directory utilizando Ansible, `realmd` e SSSD.
- Expansão do Terraform para Oracle Cloud Infrastructure (OCI).
- Padronização de configurações Windows Server.
- Desenvolvimento de roles Ansible reutilizáveis.
- Ampliação dos pipelines de CI/CD e das práticas de observabilidade.

## 💡 Filosofia do projeto

**Automatizar o que é repetitivo. Versionar o que é importante. Monitorar o que está em execução.**

Este repositório representa uma jornada contínua de evolução técnica, combinando infraestrutura tradicional com práticas modernas de DevOps.

---

**Built with curiosity, automation and a lot of troubleshooting.** 🛠️
