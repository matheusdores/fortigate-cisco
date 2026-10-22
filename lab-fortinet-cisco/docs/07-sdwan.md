# 07 — SD-WAN

## Estado atual
SD-WAN está em estudo/validação. SLA, seleção de caminho e failover não devem ser marcados como concluídos sem testes e evidências.

## Plano de validação
- [ ] Confirmar membros e interfaces WAN.
- [ ] Confirmar health-check/SLA, destinos, intervalos e limiares.
- [ ] Confirmar regra SD-WAN e critérios de seleção.
- [ ] Registrar estado normal dos links.
- [ ] Simular indisponibilidade de um link em ambiente controlado.
- [ ] Verificar mudança de caminho e continuidade/recuperação.
- [ ] Restaurar o link e registrar o comportamento de retorno.
- [ ] Repetir teste com origem em host interno.

Anexar capturas da configuração, estado do health-check, rota selecionada e resultados antes/durante/depois da falha.
