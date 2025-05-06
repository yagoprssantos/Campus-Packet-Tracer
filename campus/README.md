# Estrutura de Rede – Campus Único

## Sumário

- [Descrição da Imagem](#descrição-da-imagem)
- [Componentes e Funções](#componentes-e-sua-função)
- [Fluxo e Integração dos Componentes](#fluxo-e-integração-dos-componentes)
- [Detalhamento do Endereçamento IP](#endereçamento-ip---campus-a)

## Descrição da Imagem

Esta representação ilustra a estrutura simplificada de rede de um único campus do Centro Universitário.  
O objetivo é demonstrar de forma clara como os dispositivos e segmentos se interligam para garantir uma comunicação eficaz e o compartilhamento de recursos, sempre prezando por desempenho e segurança.

## Componentes e Sua Função

| Componente           | Função                                                                                      |
| -------------------- | ------------------------------------------------------------------------------------------- |
| **Roteador**         | Ponto de entrada e saída da rede, gerencia o tráfego e conecta o campus a redes externas.   |
| **Switch Principal** | Distribui a conexão do roteador para dispositivos locais como servidores e computadores.    |
| **Servidor**         | Centraliza aplicações, serviços e compartilhamento de arquivos para a comunidade acadêmica. |
| **Impressora**       | Oferece serviços de impressão conectada diretamente ao switch.                              |
| **Computadores**     | Garantem acesso rápido e seguro à rede para atividades acadêmicas e administrativas.        |
| **Ponto de Acesso**  | Proporciona conectividade sem fio para dispositivos móveis.                                 |
| **Notebooks**        | Utilizam Wi-Fi para mobilidade e flexibilidade no acesso à rede.                            |

## Fluxo e Integração dos Componentes

1. O **roteador** gerencia o tráfego de dados e direciona as conexões.
2. O **switch principal** distribui a conexão para os dispositivos conectados.
3. O **servidor** centraliza serviços e otimiza o fluxo de informações.
4. O **ponto de acesso** expande a conectividade para dispositivos móveis.
5. A **impressora** integra-se ao ambiente de trabalho, promovendo produtividade.
6. **Notebooks** conectados via Wi-Fi permitem mobilidade para alunos e professores.

## Endereçamento IP - Campus A

| Dispositivo                           | Endereço IP          |
| ------------------------------------- | -------------------- |
| **Roteador**                          | `192.168.10.0`       |
| **Servidor**                          | `192.168.10.10`      |
| **Impressora**                        | `192.168.10.20`      |
| **Computadores (Alunos/Professores)** | `192.168.10.101-121` |
| **Notebooks (via DHCP)**              | Atribuição dinâmica  |

> **Nota:** Este esquema de endereçamento IP foi projetado para garantir organização e facilitar a administração dos recursos de rede no Campus A.

---
