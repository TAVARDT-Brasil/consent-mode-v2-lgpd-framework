# Framework Consent Mode v2 & Conformidade LGPD | TAVARDT Brasil

[![Escopo de Verificação Perimetral](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
[![Jurisdi%C3%A7%C3%A3o](https://img.shields.io/badge/Jurisdi%C3%A7%C3%A3o-Brasil-00C853.svg)](https://ag.tavardt.com/br/ciberseguranca/)

Implementação técnica do Google Consent Mode v2, bloqueio prévio de scripts de rastreamento e conformidade técnica com as diretrizes da ANPD e da LGPD no Brasil.

Desenvolvido e mantido pela divisão de cibersegurança e proteção de infraestruturas da **[TAVARDT Brasil](https://ag.tavardt.com/br/)**.

---

## 1. Ordem de Execução e Arquitetura

Para garantir a conformidade estrita com a LGPD, insira este script no <head> da aplicação antes de carregar o Google Tag Manager:

```html
<script src="consent-mode-v2.js"></script>
<!-- O contentor do Google Tag Manager ou scripts de medicao seguem aqui -->
```

---

## 2. Recursos Técnicos Implementados

* **Estado 'Denied' por Padrão:** Bloqueia previamente o armazenamento de publicidade e analytics até ação expressa do usuário.
* **API de Atualização de Consentimento:** Disponibiliza o método window.tavardtUpdateConsent() disparando o evento tavardt_consent_updated.
* **Redação de Dados de Cliques:** Ativa ads_data_redaction para remover identificadores (GCLID/DCLID) quando o consentimento não é concedido.
* **Passagem Segura de Parâmetros:** Utiliza url_passthrough com hashes criptográficos sem persistência de cookies no navegador.

---

## 3. Documentação e Checklist de Conformidade

Consulte a lista detalhada de requisitos técnicos para o Brasil:

* [Checklist](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)

---

## 4. Ferramentas Técnicas Online (Brasil)

Audite a infraestrutura pública das suas aplicações utilizando a suíte de diagnósticos da TAVARDT:

* [Validador de Consent Mode v2 e LGPD](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
* [Auditoria de Cabeçalhos de Segurança](https://tools.tavardt.com/br/analise-cabecalhos-seguranca/)
* [Verificador DMARC e Segurança de E-mail](https://tools.tavardt.com/br/verificador-dmarc-email/)
* [Varredura de Arquivos Sensíveis Expostos](https://tools.tavardt.com/br/verificador-arquivos-expostos/)
* [Portal Completo de Ferramentas Técnicas](https://tools.tavardt.com/br/)

---

## 5. Consultoria e Remediação Técnica

Para auditorias completas de tagueamento, adequação regulatória à LGPD e consultoria avançada em consentimento no Brasil, contate a **[TAVARDT Brasil](https://ag.tavardt.com/br/contato/)**.
