# 08 — Testes e validação

| ID | Teste | Resultado conhecido | Próxima ação |
|---|---|---|---|
| T01 | OSPF core–FortiGate | FULL relatado | Anexar saída real |
| T02 | Ping core–firewall | Sem perda relatada | Registrar contagem de pacotes |
| T03 | FortiGate → gateways WAN | Resposta relatada | Registrar gateways e interfaces |
| T04 | FortiGate → 8.8.8.8 | Resposta relatada | Registrar perda, latência e rota |
| T05 | NAT nos dois ISPs | Ativo, segundo relato | Anexar configuração/sessão |
| T06 | FortiManager ↔ firewalls | Comunicação relatada | Confirmar autorização, ADOM e sincronização |
| T07 | HSRP VLAN 200 | Pendente | Investigar dois peers Active |
| T08 | Host interno → Internet | Não confirmado amplamente | Testar cada VLAN e DNS |
| T09 | SD-WAN SLA/failover | Pendente | Executar teste controlado |
| T10 | EtherChannel | Não implementado/estudo | Documentar depois de implementar |

## Modelo de registro
```text
ID:
Data/hora:
Origem:
Destino:
Comando/procedimento:
Resultado esperado:
Resultado observado:
Pacotes enviados/recebidos/perdidos:
Hipótese/causa:
Ação corretiva:
Resultado após correção:
Evidência:
Status: Pendente / Passou / Falhou / Inconclusivo
```

Não marcar um teste como aprovado sem resultado observado. Remover segredos das capturas.
