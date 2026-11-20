# Framework Consent Mode v2 & Conformidade LGPD | TAVARDT Brasil

[![Validador de Consentimento](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
[![Conformidade](https://img.shields.io/badge/Jurisdi%C3%A7%C3%A3o-Brasil-00C853.svg)](https://ag.tavardt.com/br/ciberseguranca/)

Implementação técnica do Google Consent Mode v2, bloqueio prévio de scripts de rastreamento e conformidade técnica com as diretrizes da ANPD e da LGPD no Brasil.

Desenvolvido e mantido pela divisão de privacidade digital e engenharia de dados da **[TAVARDT Brasil](https://ag.tavardt.com/br/)**.

---

## 1. Ordem de Execução e Arquitetura

Para garantir a conformidade estrita com a LGPD, este script deve ser inserido no <head> da sua aplicação imediatamente antes do carregamento do contêiner do Google Tag Manager ou scripts de medição:

```html
<script src="consent-mode-v2.js"></script>
<!-- O contentor do Google Tag Manager ou scripts de medição seguem aqui -->
```

---

## 2. Recursos Técnicos Implementados

* **Estado 'Denied' por Padrão:** Bloqueia previamente o armazenamento de publicidade e analytics até ação expressa do usuário.
* **API de Atualização de Consentimento:** Disponibiliza o método window.tavardtUpdateConsent() disparando o evento tavardt_consent_updated.
* **Redação de Dados de Cliques:** Ativa ads_data_redaction para remover identificadores (GCLID/DCLID) quando o consentimento não é concedido.
* **Passagem Segura de Parâmetros:** Utiliza url_passthrough com hashes criptográficos sem persistência de cookies no navegador.

---

## 3. Documentação e Checklist de Conformidade

Consulte a lista detalhada de requisitos técnicos para este país:

* [Checklist Técnico de Conformidade](checklist.md)

---

## 4. Ferramentas Técnicas Online (Brasil)

Audite a conformidade das suas etiquetas e proteja o seu domínio com ferramentas online verificadas:

* [Validador de Consent Mode v2 e LGPD](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
* [Auditoria de Cabeçalhos de Segurança](https://tools.tavardt.com/br/analise-cabecalhos-seguranca/)
* [Verificador DMARC e Segurança de E-mail](https://tools.tavardt.com/br/verificador-dmarc-email/)
* [Varredura de Arquivos Sensíveis Expostos](https://tools.tavardt.com/br/verificador-arquivos-expostos/)
* [Portal Completo de Ferramentas Técnicas](https://tools.tavardt.com/br/)

---

## 5. Consultoria e Governança de Tags

Para auditorias completas de tagueamento, adequação regulatória à LGPD e consultoria avançada em consentimento no Brasil, contate a **[TAVARDT Brasil](https://ag.tavardt.com/br/contato/)**.
