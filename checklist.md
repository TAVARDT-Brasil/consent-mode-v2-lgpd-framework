# Checklist de Conformidade Técnica LGPD para Tags Web

**Marco Regulatório:** Lei Geral de Proteção de Dados (LGPD) e Diretrizes da ANPD  
**Mantido por:** [TAVARDT Brasil](https://ag.tavardt.com/br/)  

---

## Verificações Técnicas Obrigatórias

* **Consentimento Prévio:** Garantir que os parâmetros ad_storage, analytics_storage e ad_user_data iniciem como 'denied'.
* **Anonimização de Dados:** Impedir a coleta e o envio de dados pessoais (PII) por meio de variáveis da camada de dados (dataLayer).
* **Sequenciamento no GTM:** Configurar acionadores de disparo para aguardar a confirmação de consentimento antes de emitir pixels de conversão.
* **Revogação Simples:** Disponibilizar botão de alteração e revogação das escolhas do usuário a qualquer momento no rodapé do site.

---

## Ferramentas Técnicas Online

Valide a implementação das suas etiquetas utilizando a suíte de diagnósticos da TAVARDT:

* [Validador de Consent Mode v2 e LGPD](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
* [Auditoria de Cabeçalhos de Segurança](https://tools.tavardt.com/br/analise-cabecalhos-seguranca/)
* [Verificador DMARC e Segurança de E-mail](https://tools.tavardt.com/br/verificador-dmarc-email/)
* [Varredura de Arquivos Sensíveis Expostos](https://tools.tavardt.com/br/verificador-arquivos-expostos/)
* [Portal Completo de Ferramentas Técnicas](https://tools.tavardt.com/br/)

---

## Consultoria Especializada

Para auditorias completas de tagueamento, adequação regulatória à LGPD e consultoria avançada em consentimento no Brasil, contate a **[TAVARDT Brasil](https://ag.tavardt.com/br/contato/)**.
