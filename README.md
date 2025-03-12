# ISP-Network-Design
Planeamento, desenho e configuração de uma rede interligada de ISPs com conectividade empresarial e acesso à Internet, utilizando GNS3.

Este repositório documenta o desenvolvimento de uma solução de rede, no âmbito de um projeto da unidade curricular de Redes de Computadores, no 3.º ano do curso de Engenharia Informática. O objetivo do projeto foi planear, desenhar, configurar e documentar uma rede formada por vários ISPs interligados, com especial foco em otimizar a conectividade e garantir redundância, escalabilidade e qualidade de serviço (QoS). A rede foi desenhada e configurada utilizando a ferramenta GNS3, com as seguintes considerações:

A rede é composta por ISPs de diferentes níveis (Tier 1, Tier 2 e Tier 3), onde o tráfego entre as diferentes camadas é gerido de forma redundante e otimizada.
A configuração do endereçamento foi realizada de forma a garantir uma utilização adequada para IPv4 e IPv6, com a implementação de endereços link-local em todas as interfaces com IPv6.
O ISP Tier 3A foi configurado com OSPF em um ambiente multi-área, com tabelas de encaminhamento otimizadas.
A implementação do BGP no ISP Tier 3A foi projetada para reduzir o número de ligações iBGP através do uso de confederações.
Foi garantida a redundância das ligações entre o Tier 3A e os Tier 2, com o uso paralelo dos links.
A QoS foi implementada no Tier 3A e no cliente empresarial para garantir o tráfego prioritário.
A conectividade do cliente empresarial foi configurada com VPN L3 sobre tecnologia MPLS, garantindo a ligação segura entre a Sede e as Filiais, com protocolos diferentes para as ligações entre a rede do cliente e os routers PE dos operadores.
A conectividade à Internet para o cliente foi assegurada através do router da Sede.
Além disso, a solução garante a implementação de políticas de tráfego entre os diferentes ISPs e foi testada para garantir que as necessidades da rede empresarial e os requisitos de redundância e performance foram atendidos.

