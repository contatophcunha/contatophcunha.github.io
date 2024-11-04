---
title: "FLASK APP"
date: 2024-09-12 13:13:13 +351
categories: [APPS]
tags: [FLASK]
---
# Preparando um Laboratório Prático de Kubernetes com Podtato-Head 🚀

Neste post, compartilho uma experiência prática que será útil para quem deseja aprender Kubernetes de forma prática e descomplicada. Através do projeto Podtato-Head, configurei um ambiente local com Docker Desktop e Kubernetes no Ubuntu, e vou detalhar o passo a passo que segui para iniciar essa jornada!

## Configurando o Ambiente

### 1. Instalando Docker Desktop no Ubuntu

O Docker Desktop é uma ótima escolha para gerenciar containers localmente, pois oferece a opção de habilitar o Kubernetes diretamente em sua interface.

#### Baixando e Instalando o Docker Desktop:

```bash
sudo apt update
sudo apt install ./docker-desktop-<version>-<arch>.deb


```

####	Habilitando Kubernetes:
Após a instalação, acesse as configurações do Docker Desktop e ative o Kubernetes. Isso permite iniciar um cluster Kubernetes local e experimentar aplicações distribuídas de forma simples e rápida.

### 2. Configurando o Repositório Podtato-Head

Com o ambiente pronto, é hora de configurar o Podtato-Head, uma aplicação de exemplo projetada para ilustrar conceitos de microserviços.

```bash
git clone https://github.com/podtato-head/podtato-head.git
cd podtato-head
```
 Com o repositório configurado, você já pode aplicar os manifests do Kubernetes para fazer o primeiro deploy, que seguirá nos passos abaixo após uma visão geral das tecnologias utilizadas no projeto.


####	Explorando Tecnologias no Lab Kubernetes com Podtato-Head:

Este laboratório proporciona uma visão prática de tecnologias interconectadas, como Docker, Kubernetes e microserviços. Aqui estão as principais ferramentas que você utilizará:

1.	Kubernetes 🌐
Kubernetes, ou K8s, é uma plataforma de orquestração de containers. Ele gerencia os pods, garantindo escalabilidade e alta disponibilidade para os microserviços do Podtato-Head.

2.	Docker 🐳
Docker permite criar e executar containers para cada microserviço do Podtato-Head, simplificando o desenvolvimento e a execução local.

3.	Microserviços 🧩
O Podtato-Head é dividido em vários microserviços (cada parte como olhos, boca e braços é um container separado), que comunicam-se por meio de APIs.

4.	Helm 🎛️
Utilizaremos Helm para facilitar o deploy da aplicação Podtato-Head no Kubernetes com um gerenciamento de dependências e configurações centralizado.

5.	Prometheus e Grafana 📊
Prometheus coleta métricas dos containers, enquanto o Grafana cria dashboards para visualização e monitoramento.

6.	Service Mesh (Istio/Linkerd) 🔀
Uma camada de Service Mesh como Istio ajuda a gerenciar o tráfego entre microserviços, oferecendo segurança e controle avançado sobre as conexões.

7.	CI/CD (Jenkins/GitLab) 🔄
A integração com CI/CD permite a automação de build e deploy dos microserviços, mantendo o fluxo de atualizações contínuas.


