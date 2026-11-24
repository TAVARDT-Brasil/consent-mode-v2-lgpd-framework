# Framework Consent Mode v2 & Conformidade LGPD | TAVARDT Brasil

[![Diagn%C3%B3stico%20T%C3%A9cnico](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/br/validador-consent-mode-v2-lgpd/)
Implementação técnica do Google Consent Mode v2, bloqueio prévio de scripts de rastreamento e conformidade técnica com a LGPD e resoluções da ANPD no Brasil.

Desenvolvido e mantido pela divisão de cibersegurança e proteção de dados da **TAVARDT Brasil**.

***

## 1. Ordem de Execução e Arquitetura

Para garantir a conformidade estrita com a LGPD, insira este script no <head> da aplicação antes de carregar o Google Tag Manager:

```html
<script src="consent-mode-v2.js"></script>
<!- Google Tag Manager / measurement scripts execute here ->
```

***

## 2. Recursos Técnicos Implementados

* **Estado Padrão Negado (Default Denied):** ad_storage, analytics_storage e ad_user_data iniciam estritamente como negados.
* **API de Atualização Orientada a Eventos:** Função global window.tavardtConsent.update() sincronizada com o dataLayer.
* **Redação Automática de Parâmetros de Anúncios:** Ativação nativa de ads_data_redaction para supressão de identificadores.
* **Preservação de Tráfego sem Cookies:** Ativação de url_passthrough para atribuição analítica anônima sem persistência local.

***

## 3. Documentação e Checklist de Conformidade

Consulte a lista detalhada de requisitos técnicos para o Brasil:

* Checklist

***

## 4. Ferramentas Técnicas Online (Brasil)

Audite a infraestrutura pública das suas aplicações utilizando a suíte de diagnósticos da TAVARDT:

* Validador de Consent Mode v2 e LGPD
* [Auditoria de Cabeçalhos de Segurança](https://tools.tavardt.com/br/analise-cabecalhos-seguranca/)
* [Verificador DMARC e Autenticação](https://tools.tavardt.com/br/verificador-dmarc-email/)
* [Verificador de Arquivos Expostos](https://tools.tavardt.com/br/verificador-arquivos-expostos/)
* [Portal de Diagnóstico Técnico Brasil](https://tools.tavardt.com/br/)

***

## 5. Consultoria e Remediação Técnica

Para auditorias periciais de tags, validação de CMPs e adequação de privacidade no Brasil, entre em contato com a **TAVARDT Brasil**.
