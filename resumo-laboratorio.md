## Gerenciamento de Instâncias EC2 na AWS

O Amazon EC2 é um serviço da AWS que permite criar e gerenciar máquinas virtuais na nuvem. Essas máquinas virtuais, chamadas de instâncias, podem executar sistemas operacionais como Linux ou Windows e serem utilizadas para hospedar aplicações, testar sistemas, executar scripts, armazenar dados temporários e simular ambientes computacionais.

No contexto do laboratório, o gerenciamento de instâncias EC2 envolve atividades como selecionar uma AMI, configurar uma instância, definir o tipo de máquina, associar armazenamento EBS, configurar regras de acesso e, ao final, parar ou encerrar os recursos para evitar custos desnecessários.

## AMI - Amazon Machine Image

Uma AMI é uma imagem utilizada como modelo para criar uma instância EC2. Ela pode conter o sistema operacional, configurações, aplicações instaladas e outros ajustes necessários para iniciar uma máquina virtual.

Na prática, a AMI funciona como um “molde” de uma máquina já configurada. Isso permite criar novas instâncias com o mesmo padrão, evitando repetir manualmente toda a instalação e configuração do ambiente.

Em um cenário de automação, uma AMI poderia ser usada para padronizar ambientes de teste, servidores de supervisão, aplicações industriais, sistemas de coleta de dados ou plataformas de análise conectadas a sensores e controladores.

## EBS - Elastic Block Store

O Amazon EBS é um serviço de armazenamento em bloco utilizado pelas instâncias EC2. Ele funciona como um disco virtual, semelhante a um HD ou SSD, que pode armazenar o sistema operacional, arquivos, aplicações e dados utilizados pela instância.

Uma característica importante do EBS é que os dados podem continuar existindo mesmo quando a instância EC2 é parada, dependendo da configuração utilizada. Isso é útil quando é necessário preservar informações ou restaurar um ambiente posteriormente.

## Snapshot EBS

O snapshot é uma cópia de segurança de um volume EBS. Ele permite salvar o estado do disco em determinado momento, funcionando como um backup.

Esse recurso é importante para recuperação de dados, migração de ambientes e proteção contra falhas. Caso uma instância apresente problema, é possível restaurar um volume a partir do snapshot e recuperar informações anteriores.

## Aplicação em Engenharia de Controle e Automação

Na Engenharia de Controle e Automação, recursos como EC2, AMI e Snapshot EBS podem ser aplicados em ambientes que envolvem coleta, processamento e análise de dados industriais.

Por exemplo, uma instância EC2 pode ser utilizada para hospedar uma aplicação responsável por receber dados de sensores, armazenar informações de processos, executar dashboards, realizar análises com Python ou integrar sistemas industriais com serviços em nuvem.

A AMI pode ser usada para criar um ambiente padrão contendo ferramentas já instaladas, como bibliotecas de análise de dados, softwares de monitoramento, scripts de automação ou serviços de comunicação. Dessa forma, caso seja necessário criar uma nova máquina, ela já nasce configurada com o ambiente adequado.

O Snapshot EBS, por sua vez, pode ser usado como estratégia de backup. Em sistemas industriais, a perda de dados pode prejudicar análises, relatórios e históricos de operação. Por isso, manter cópias dos volumes ajuda na recuperação em caso de erro, falha ou necessidade de migração.

## Exemplo prático de uso

Imagine um sistema de monitoramento de temperatura de um forno industrial. Os dados dos sensores poderiam ser enviados para uma aplicação hospedada em uma instância EC2. Essa aplicação poderia processar os dados, gerar gráficos, armazenar históricos e auxiliar na tomada de decisão.

Nesse cenário:

- a EC2 funcionaria como o servidor da aplicação;
- o EBS funcionaria como o disco onde os dados e arquivos ficam armazenados;
- o Snapshot EBS funcionaria como backup do ambiente;
- a AMI permitiria criar uma nova instância já configurada, caso fosse necessário replicar ou restaurar o sistema.

## Cuidados importantes

Ao utilizar instâncias EC2, é importante entender a responsabilidade compartilhada na nuvem. A AWS é responsável pela infraestrutura física, como datacenters, servidores, energia e rede física. Já o usuário é responsável por configurar o sistema operacional, gerenciar aplicações, controlar acessos e proteger os dados.

Também é importante parar ou encerrar instâncias que não estão sendo utilizadas, além de remover volumes, snapshots e AMIs desnecessários, pois esses recursos podem gerar custos na conta AWS.

## Conclusão

O laboratório permitiu compreender como a AWS pode ser utilizada para criar e gerenciar ambientes computacionais na nuvem. Os conceitos de EC2, AMI, EBS e Snapshot são importantes para criar máquinas virtuais, padronizar ambientes, realizar backups e garantir maior segurança na recuperação de dados.

Na área de Controle e Automação, esses recursos podem apoiar aplicações voltadas ao monitoramento industrial, análise de dados, integração com sensores, supervisão de processos e desenvolvimento de soluções conectadas à nuvem.
