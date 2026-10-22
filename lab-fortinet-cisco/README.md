# Fortinet + Cisco Homelab

Documentação de um laboratório de redes e segurança com dois FortiGate, FortiManager, switches Cisco e dois ISPs simulados (Vivo e Claro).

> **Status:** documentação inicial baseada nos resultados relatados durante o laboratório. Itens ainda não verificados permanecem explicitamente como pendências.

## Ambiente
- 2 FortiGate com FortiOS 7.2.4, em modo standalone no cenário atual.
- FortiManager para gestão centralizada.
- Switching Cisco com VLANs e STP.
- OSPF entre core e FortiGate.
- HSRP na VLAN 200 em investigação.
- Dois ISPs simulados: Vivo e Claro.
- SD-WAN em validação.
- EtherChannel: tópico de estudo, ainda não considerado implementado.

## Resultados relatados
- Adjacência OSPF em estado `FULL` entre core e FortiGate.
- Ping sem perda nos links entre core e firewall.
- FortiGate alcançando gateways dos ISPs e recebendo resposta de `8.8.8.8`.
- NAT dinâmico ativo nos dois ISPs.
- Acesso ao FortiManager e comunicação com os dois firewalls.

## Pendências principais
- Investigar os dois cores observados em estado HSRP `Active` na VLAN 200.
- Confirmar rotas padrão nos cores e rotas de retorno para as VLANs internas.
- Testar Internet a partir de clientes internos, com quantidade fixa de pacotes.
- Validar SLA e failover do SD-WAN com evidências.
- Confirmar autorização, ADOM e sincronização de configuração no FortiManager.

## Índice
- [Topologia](docs/01-topologia.md)
- [VLANs, switching e STP](docs/02-vlans-switching-stp.md)
- [OSPF e roteamento](docs/03-ospf-routing.md)
- [HSRP e redundância](docs/04-hsrp-redundancia.md)
- [FortiGate, NAT e ISPs](docs/05-fortigate-nat-isp.md)
- [FortiManager](docs/06-fortimanager.md)
- [SD-WAN](docs/07-sdwan.md)
- [Testes e validação](docs/08-testes-e-validacao.md)
- [Pendências](docs/09-pendencias.md)

## Evidências
Adicione capturas reais e configurações sanitizadas em pastas `images/` e `configs/`. Antes de publicar, remova senhas, tokens, chaves privadas e dados sensíveis. Não versionar configuração de produção nem afirmar como concluído um teste sem evidência.
