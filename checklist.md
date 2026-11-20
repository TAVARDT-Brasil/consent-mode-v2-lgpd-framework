# Checklist de Conformidade Técnica LGPD para Tags

**Regulatory Standard:** Lei Geral de Proteção de Dados (LGPD) e Diretrizes ANPD  
**Maintained by:** [TAVARDT Brasil](https://ag.tavardt.com/br/)  

---

## Technical Audit Points

* **Consentimento Prévio:** Configurar todos os parâmetros de publicidade e analytics com 'denied' antes de qualquer interação do usuário.
* **Anonimização de IP:** Forçar a remoção de identificadores pessoais antes do despacho para servidores externos.
* **Redação de Dados de Anúncios:** Ativar ads_data_redaction para remover identificadores de cliques quando o consentimento for negado.
* **Sequenciamento no GTM:** Garantir que tags de mídia paga disparem estritamente após o evento de atualização de consentimento.

---

## Online Verification Tools

Validate your tag deployment and perimeter security using TAVARDT diagnostic suites:

* [HTTP Security Headers Checker](https://tools.tavardt.com/br/security-headers-check/)
* [Exposed Secret & Credential Scanner](https://tools.tavardt.com/br/exposed-files-scanner/)
* [Full Diagnostic Suite](https://tools.tavardt.com/br/)

For professional privacy architecture, tag auditing, and CRO optimization, contact [TAVARDT Brasil](https://ag.tavardt.com/br/contact/).
