# Estrutura de Rede – Campus Único

## Sumário

- [Descrição da Imagem](#descrição-da-imagem)
- [Componentes e Funções](#componentes-e-sua-função)
- [Fluxo e Integração dos Componentes](#fluxo-e-integração-dos-componentes)
- [Detalhamento do Endereçamento IP](#endereçamento-ip---campus-a)
- [Estratégia de Segmentação da Rede](#estratégia-de-segmentação-da-rede)
- [Estratégias de Implementação](#estratégias-de-implementação)
- [Topologia e Conectividade](#topologia-e-conectividade)
- [Configurações de Segurança](#configurações-de-segurança)
- [Detalhamento do Endereçamento IP](#detalhamento-do-endereçamento-ip)
- [Considerações de Implementação](#considerações-de-implementação)

## Descrição da Rede

Estrutura simplificada de rede de um único campus do Centro Universitário.  
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

## Estratégia de Segmentação da Rede

A rede foi estrategicamente segmentada em diferentes grupos de usuários:

1. **Área Administrativa**

   - Servidor centralizado (192.168.10.10)
   - Impressora dedicada (192.168.10.20)
   - Outros serviços administrativos (192.168.10.30)

2. **Área Acadêmica**
   - Laboratórios de Alunos (192.168.10.101-109)
   - Computadores de Professores (192.168.10.120-122)
   - Rede Wireless para notebooks (DHCP)

## Estratégias de Implementação

1. **Segmentação Física**

   - Switch principal como ponto central de distribuição
   - Conexões dedicadas para servidor e impressora
   - Divisão de laboratórios em grupos de computadores

2. **Segmentação Lógica**
   - VLANs separadas para alunos e professores
   - Rede wireless isolada para dispositivos móveis
   - Controle de acesso baseado em grupos de usuários

## Topologia e Conectividade

1. **Hierarquia de Rede**

   - Roteador Principal (Gateway: 192.168.10.0)
   - Switch Principal (Core)
   - Access Point para rede wireless

2. **Distribuição de Equipamentos**
   - 9 computadores para alunos
   - 3 computadores para professores
   - 4 notebooks com acesso wireless
   - 1 servidor central
   - 1 impressora de rede

## Configurações de Segurança

1. **Controle de Acesso**

   - Autenticação para rede wireless
   - Separação de tráfego entre VLANs
   - Políticas de firewall no roteador

2. **Gerenciamento de Recursos**
   - QoS para aplicações críticas
   - Controle de banda por tipo de usuário
   - Monitoramento de tráfego

## Detalhamento do Endereçamento IP

| Segmento de Rede | Range de IP        | Função                          |
| ---------------- | ------------------ | ------------------------------- |
| Infraestrutura   | 192.168.10.0-30    | Equipamentos core               |
| Professores      | 192.168.10.20-50   | Computadores dos docentes       |
| Alunos (Lab)     | 192.168.10.101-109 | PCs do laboratório              |
| Rede Wireless    | DHCP (10.110-150)  | Notebooks e dispositivos móveis |

## Considerações de Implementação

- Utilização de VLANs para segregação de tráfego
- Implementação de DHCP para rede wireless
- Redundância em conexões críticas
- Monitoramento centralizado via servidor
- Backup automático de configurações
- Documentação detalhada de todas as conexões e configurações
