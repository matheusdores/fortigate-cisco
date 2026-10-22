# 05 — FortiGate, NAT e ISPs

## Resultados relatados
- FortiGate alcançou os gateways dos ISPs.
- O firewall recebeu resposta de `8.8.8.8`.
- NAT dinâmico foi relatado como ativo nos dois ISPs.

Esses testes a partir do próprio firewall não comprovam, isoladamente, acesso à Internet a partir de todas as VLANs internas.

## Comandos de coleta FortiGate
```text
get router info routing-table all
show system interface
show firewall policy
show firewall central-snat-map
diagnose sys session list
```

O comando de Central SNAT só é pertinente se esse recurso for usado; verificar a configuração real e preferir o método de NAT que corresponde ao ambiente.

## Checklist
- [ ] Confirmar interfaces WAN e gateways.
- [ ] Confirmar rota padrão e distância/prioridade.
- [ ] Identificar policy de saída e interfaces.
- [ ] Confirmar método NAT configurado.
- [ ] Testar cada VLAN a partir de um host interno.
- [ ] Confirmar rota de retorno e DNS.
- [ ] Guardar evidências com dados sensíveis removidos.
