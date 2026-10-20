# 🔐 Pentest Web — VulnBank

## 📌 Sobre o projeto
Este repositório apresenta um relatório técnico de **Pentest Web** realizado na aplicação bancária de treinamento **VulnBank**, em outubro de 2026.

O objetivo foi identificar, testar e documentar vulnerabilidades, compreender seus impactos e propor melhorias de segurança. O relatório reúne etapas de reconhecimento, análise de requisições, testes de autenticação e autorização, evidências e recomendações.

## 🛠️ Ferramentas utilizadas
- **Kali Linux** — ambiente de testes.
- **Burp Suite** — interceptação e análise de requisições HTTP.
- **Gobuster** — enumeração de diretórios e recursos.
- **cURL** — inspeção de respostas HTTP.
- **John the Ripper** — análise da resistência de assinaturas JWT.

## 🔎 Principais vulnerabilidades documentadas

| Vulnerabilidade | Impacto observado ou analisado |
| --- | --- |
| Mass Assignment | Criação indevida de conta com privilégios administrativos. |
| JWT inseguro | Fragilidades na assinatura e no gerenciamento de tokens. |
| IDOR | Acesso indevido a dados e transações de outros usuários. |
| Cross-Site Scripting (XSS) | Injeção de conteúdo não sanitizado em funcionalidades web. |
| Server-Side Request Forgery (SSRF) | Requisições do servidor a recursos internos. |
| Information Disclosure | Exposição de detalhes internos e mensagens de erro. |
| Werkzeug Debugger exposto | Interface de depuração acessível, com risco de exploração adicional. |

## 📊 Resultados
Os testes registrados no relatório demonstraram falhas relevantes de autenticação, autorização e validação de dados, incluindo elevação de privilégios, acesso indevido a informações financeiras e manipulação não autorizada de transações.

A avaliação final do relatório classifica o cenário como **crítico** e recomenda priorizar a proteção do debugger, o fortalecimento dos JWTs, a validação de permissões em cada endpoint e o tratamento seguro das entradas e respostas.

## 🎯 Conhecimentos aplicados
- Reconhecimento e enumeração de aplicações web
- Análise de tráfego HTTP e APIs
- Testes de autenticação e controle de acesso
- Identificação de vulnerabilidades web
- Análise de riscos e documentação técnica

## 📄 Relatório completo
Consulte o arquivo PDF deste repositório para acompanhar as evidências, os procedimentos e as recomendações detalhadas.

## ⚠️ Uso responsável
Projeto de finalidade educacional. Testes de segurança devem ser realizados apenas em ambientes próprios, de treinamento ou expressamente autorizados.

---
**Autor:** Guilherme Isidoro Possamai  
**Data:** Outubro de 2026  
**Área:** Cibersegurança · Pentest Web · Segurança Ofensiva
