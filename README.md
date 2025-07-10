# 🌐 Guia Introdutório: Monitoramento de Recursos no Azure (com foco em VMs)

Bem-vindo ao seu primeiro passo no universo do Microsoft Azure!  
Este repositório tem como objetivo te ajudar a entender e configurar o **monitoramento de recursos no Azure**, especialmente **máquinas virtuais (VMs)**, de forma simples, prática e eficiente.

---

## ✅ 1. Introdução ao Monitoramento no Azure

O monitoramento permite acompanhar o desempenho e detectar eventos importantes no ambiente de nuvem. No caso das VMs, ele ajuda a visualizar uso de CPU, disco, rede e ações administrativas como exclusão.

**Ferramentas principais:**

- Azure Monitor  
- Log Analytics  
- Alertas  
- Activity Log

---

## 🛠️ 2. Etapas práticas para configurar o monitoramento

### 🔹 Etapa 1: Acessar o painel de monitoramento

No portal do Azure, acesse sua VM e clique em **"Monitoramento"** no menu lateral.

![Painel de Monitoramento da VM](images/portal_vm_monitor.png)

---

### 🔹 Etapa 2: Habilitar Log Analytics

Se a opção de insights não estiver ativa, habilite e conecte a um workspace.

![Habilitar Log Analytics](images/enable_log_analytics.png)

---

### 🔹 Etapa 3: Ver métricas da VM

Depois de habilitado, vá em **"Métricas"** e selecione a métrica desejada (CPU, disco etc.).

![Exemplo de Dashboard com Métricas](images/metrics_dashboard.png)

---

## 🔔 3. Como configurar alertas para eventos críticos

Para receber notificações em caso de exclusão de uma VM, crie uma **regra de alerta** baseada no **Activity Log**:

1. Vá em **Monitor > Alertas > Nova Regra**
2. Escopo: sua assinatura
3. Condição:  
   - *Operation Name* = `Delete Virtual Machine`
4. Ações: notificação por e-mail ou webhook

![Alerta para Exclusão de VM](images/alert_rule_delete_vm.png)

---

## 💡 4. Dicas e boas práticas

- Conecte a VM ao workspace de log logo após criá-la
- Use tags para organizar seus recursos
- Ative alertas para operações administrativas importantes

---

## 📚 5. Glossário rápido

| Termo             | Definição |
|------------------|-----------|
| VM               | Computador virtual |
| Azure Monitor    | Ferramenta de observabilidade |
| Log Analytics    | Coleta e análise de logs |
| Alertas          | Notificações automáticas |
| Activity Log     | Registro de ações administrativas |

---

## 📝 6. Leitura complementar

- [Documentação do Azure Monitor](https://learn.microsoft.com/pt-br/azure/azure-monitor/)
- [Configurar alertas](https://learn.microsoft.com/pt-br/azure/azure-monitor/alerts/alerts-overview)
- [Log Analytics](https://learn.microsoft.com/pt-br/azure/azure-monitor/logs/log-analytics-overview)

---
