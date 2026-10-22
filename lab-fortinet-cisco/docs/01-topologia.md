# 01 — Topologia

O laboratório integra dois FortiGate, FortiManager, switches Cisco e dois provedores WAN simulados.

## Diagrama
Adicionar o diagrama real em `../images/topologia-geral.png`.

O diagrama deve identificar equipamentos, interfaces, VLANs, redes IP, gateways, enlaces de trânsito, vizinhanças OSPF e caminho esperado de ida e volta do tráfego.

## Inventário conhecido
| Componente | Função | Estado |
|---|---|---|
| FortiGate 1 e 2 | Firewall, NAT e roteamento | Em uso |
| FortiManager | Gestão centralizada | Comunicação relatada |
| Cisco Core 1 e 2 | Switching L2/L3 e HSRP | HSRP em investigação |
| ISP Vivo (simulado) | WAN | Gateway testado, segundo relato |
| ISP Claro (simulado) | WAN | Gateway testado, segundo relato |

## Endereçamento
Preencher com os valores reais da configuração; não inferir sub-redes a partir dos nomes.

| Segmento | VLAN/rede | Gateway | Observação |
|---|---|---|---|
| VLAN 200 | Confirmar | Confirmar | HSRP pendente |
| Trânsito core–FortiGate | Confirmar | Confirmar | OSPF FULL relatado |
| WAN Vivo | Confirmar | Confirmar | Conectividade relatada |
| WAN Claro | Confirmar | Confirmar | Conectividade relatada |

## Evidências
- [ ] Diagrama validado.
- [ ] Capturas das interfaces e rotas.
- [ ] Configurações sanitizadas.
