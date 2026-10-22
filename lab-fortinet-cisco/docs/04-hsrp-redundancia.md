# 04 — HSRP e redundância

## Estado atual
HSRP na VLAN 200 está em investigação. Os dois cores foram observados como `Active`; não marcar como concluído até confirmar grupo, VLAN, IP virtual, conectividade L2 e parâmetros.

## Coleta Cisco
```text
show standby brief
show standby
show running-config
show interfaces trunk
show spanning-tree vlan 200
```

Revise e remova segredos antes de compartilhar saídas de configuração.

## Checklist
- [ ] Mesmo número de grupo nos peers.
- [ ] Mesmo IP virtual e sub-rede.
- [ ] Conectividade L2 entre os peers na VLAN.
- [ ] Comparar prioridade, preempt e timers.
- [ ] Verificar mensagens de estado e possíveis duplicidades.
- [ ] Confirmar gateway virtual único e alcançável.
- [ ] Executar failover controlado e registrar evidência.

Só concluir após registrar o estado Active/Standby esperado e um teste de failover reproduzível.
