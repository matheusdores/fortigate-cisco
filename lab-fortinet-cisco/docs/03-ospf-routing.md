# 03 — OSPF e roteamento

## Resultado relatado
A adjacência OSPF entre o core Cisco e o FortiGate foi observada em estado `FULL`. Também foram relatados pings sem perda nos links entre core e firewall.

## Comandos Cisco
```text
show ip ospf neighbor
show ip route ospf
show ip route
show ip protocols
```

## Comandos FortiGate
```text
get router info ospf neighbor
get router info routing-table all
```

A sintaxe e a disponibilidade dos comandos podem variar conforme versão e contexto.

## Critérios de validação
- Adjacência no estado esperado.
- Rotas aprendidas correspondem ao desenho.
- Próximo salto e interface de saída corretos.
- Rotas de retorno para as VLANs internas.
- Teste de ida e volta originado de host interno.

## Pendências
- [ ] Anexar saídas reais de vizinhança e tabela de rotas.
- [ ] Confirmar rotas de retorno.
- [ ] Testar conectividade de clientes internos, não apenas do firewall.
