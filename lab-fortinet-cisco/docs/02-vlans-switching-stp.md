# 02 — VLANs, switching e STP

## Objetivo
Documentar segmentação L2, portas access/trunk e prevenção de loops com Spanning Tree Protocol (STP).

O laboratório utiliza VLANs e STP, mas os IDs, portas, VLAN nativa, VLANs permitidas e modo STP devem ser confirmados nas configurações reais antes de registrar valores definitivos.

## Comandos Cisco para coleta
```text
show vlan brief
show interfaces trunk
show spanning-tree
show spanning-tree vlan <VLAN_ID>
show mac address-table dynamic
show interfaces status
```

Substitua `<VLAN_ID>` por um identificador existente.

## Checklist
- [ ] Confirmar VLANs e finalidade.
- [ ] Confirmar VLAN nativa e VLANs permitidas por trunk.
- [ ] Confirmar root bridge e modo STP.
- [ ] Verificar portas forwarding/blocking.
- [ ] Testar conectividade dentro de cada VLAN.
- [ ] Confirmar que cada VLAN chega ao gateway esperado.

Adicionar capturas reais em `../images/cisco/`. Remover dados sensíveis antes de publicar.
