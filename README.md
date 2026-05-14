# Laboratório AWS EC2 - DIO

Repositório desenvolvido para documentar conceitos e práticas de gerenciamento de instâncias EC2 na AWS, incluindo criação de AMIs, uso de volumes EBS e snapshots para backup e recuperação.

## Sobre o desafio

Este projeto faz parte de um laboratório prático da DIO com foco em conceitos fundamentais de gerenciamento de instâncias EC2 na AWS.

O objetivo principal é consolidar os conhecimentos adquiridos durante as aulas, documentando os principais conceitos estudados e relacionando-os com possíveis aplicações práticas em ambientes de tecnologia, computação em nuvem e automação.

## Tecnologias e serviços estudados

- Amazon EC2
- Amazon EBS
- Amazon Machine Image - AMI
- Snapshots EBS
- AWS Cloud
- GitHub
- Markdown

## Conceitos principais

### Amazon EC2

O Amazon EC2 é um serviço da AWS que permite criar e gerenciar máquinas virtuais na nuvem. Essas máquinas são chamadas de instâncias e podem executar sistemas operacionais como Linux ou Windows.

Na prática, uma instância EC2 funciona como um servidor virtual, que pode ser utilizado para hospedar aplicações, executar scripts, criar ambientes de teste, processar dados ou simular estruturas computacionais.

### Amazon EBS

O Amazon EBS é um serviço de armazenamento em bloco utilizado junto com instâncias EC2. Ele funciona como um disco virtual, semelhante a um HD ou SSD, onde podem ser armazenados o sistema operacional, arquivos, aplicações e dados da instância.

O volume EBS pode continuar existindo mesmo após a instância ser parada ou encerrada, dependendo da configuração escolhida.

### Snapshot EBS

O snapshot é uma cópia de segurança de um volume EBS. Ele permite salvar o estado do disco em determinado momento, funcionando como uma forma de backup.

Esse recurso é importante para recuperação de dados, migração de ambientes e proteção contra falhas.

### AMI - Amazon Machine Image

A AMI é uma imagem utilizada como modelo para criar uma instância EC2. Ela pode conter o sistema operacional, configurações, aplicações instaladas e outros ajustes necessários.

Na prática, a AMI funciona como um “molde” de uma máquina já configurada. Isso permite criar novas instâncias com o mesmo padrão, evitando a necessidade de configurar tudo manualmente novamente.

## Etapas estudadas no laboratório

Durante o laboratório, foram abordadas etapas relacionadas ao gerenciamento de instâncias EC2, como:

1. Compreensão do funcionamento de uma instância EC2.
2. Identificação do papel do armazenamento EBS.
3. Criação e utilização de snapshots para backup.
4. Entendimento da função das AMIs.
5. Relação entre instâncias, volumes, imagens e backups.
6. Cuidados necessários para evitar custos desnecessários na AWS.
7. Organização da documentação técnica em um repositório GitHub.

## Aplicação em Engenharia de Controle e Automação

Na área de Engenharia de Controle e Automação, os recursos estudados podem ser aplicados em cenários de monitoramento, análise de dados e integração de sistemas industriais com a nuvem.

Por exemplo, uma instância EC2 poderia hospedar uma aplicação responsável por receber dados de sensores, processar informações de um sistema de supervisão, gerar dashboards ou executar scripts de análise.

Nesse contexto:

- A EC2 funcionaria como o servidor virtual da aplicação.
- O EBS armazenaria arquivos, dados e configurações.
- O snapshot permitiria criar backups do ambiente.
- A AMI permitiria replicar uma máquina já configurada.

Um exemplo prático seria um sistema de monitoramento de temperatura de um forno industrial. Os dados poderiam ser enviados para uma aplicação hospedada em uma instância EC2, permitindo análise, armazenamento histórico e apoio na tomada de decisão.

## Responsabilidade compartilhada

Ao utilizar serviços em nuvem, é importante compreender o modelo de responsabilidade compartilhada.

A AWS é responsável pela infraestrutura física, como datacenters, servidores, energia, refrigeração e rede física.

O cliente é responsável por configurar e proteger o ambiente utilizado, incluindo sistema operacional, aplicações, permissões de acesso, dados e boas práticas de segurança.

## Cuidados com custos

Durante o uso da AWS, é importante verificar quais recursos estão ativos para evitar cobranças inesperadas.

Alguns cuidados importantes são:

- Encerrar instâncias EC2 que não estão sendo utilizadas.
- Excluir volumes EBS desnecessários.
- Remover snapshots antigos que não serão mais usados.
- Excluir AMIs criadas apenas para testes.
- Acompanhar o painel de cobrança da AWS.
- Utilizar recursos dentro dos limites gratuitos quando disponíveis.

## Organização do repositório

```text
lab-ec2-aws-dio/
│
├── README.md
├── resumo-laboratorio.md
└── referencias.md
