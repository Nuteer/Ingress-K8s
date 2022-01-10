# Ingress-K8s

# Tutorial para instalação, configuração e teste de INGRESS-NGINX

## Pré-requisito

Um cluster kubernetes instalado e configurado

## Como instalar o Ingress

foi utilizado a documetação oficial do [INGRESS-NGINX].  

Como estou utilizando um ambiente Bare-Metal, segue os pre-requisitos gerais e o especifico para bare-metal, onde fez o deploy por nodePort

## Sobre o teste

O teste tem o objetivo de validar o roteamento do ingress entre os deploys de duas aplicações.

## Deploy do teste

Com o [INGRESS-NGINX] funcionando, efetue o deploy das duas aplicações
```
kubectl apply -f ./k8s/blue-deployment.yaml
kubectl apply -f ./k8s/green-deployment.yaml
```
Verifique se os deploys estão funcionando
