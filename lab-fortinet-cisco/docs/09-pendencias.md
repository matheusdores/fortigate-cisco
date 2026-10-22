# 09 — Pendências e próximos passos

## Roteamento e redundância
- [ ] Investigar dois cores em estado HSRP `Active` na VLAN 200.
- [ ] Confirmar rotas padrão nos cores.
- [ ] Confirmar rotas de retorno para VLANs internas.
- [ ] Testar host interno até destinos externos, incluindo DNS.

## WAN e SD-WAN
- [ ] Repetir testes com quantidade fixa de pacotes.
- [ ] Registrar perda e latência por ISP.
- [ ] Validar health-check/SLA.
- [ ] Testar failover e retorno ao link.

## FortiManager
- [ ] Confirmar autorização, ADOM e sincronização dos dois FortiGate.
- [ ] Registrar versões e evidências.

## Documentação
- [ ] Adicionar diagrama real em `images/`.
- [ ] Adicionar capturas reais em `images/`.
- [ ] Exportar configurações sanitizadas para `configs/`.
- [ ] Estudar e validar EtherChannel em etapa separada.
- [ ] Atualizar o README após cada teste.

## Critério para fechar pendência
Registrar configuração aplicada, teste reproduzível, resultado observado e evidência. Até lá, manter pendente.
