# Análise de Incidente DDoS e Proposta de Fortalecimento de Rede

<div align="right">
<a href="./README.md">View in English 🇺🇸</a>
</div>

## Visão Geral do Projeto

Um estudo de caso prático desenvolvido como parte do [Certificado Profissional de Cibersegurança do Google](https://www.coursera.org/google-certificates/cybersecurity-certificate), focado na análise de um incidente de segurança e na aplicação do Framework de Cibersegurança do NIST para guiar a resposta. O objetivo foi analisar um ataque DDoS (Distributed Denial of Service), identificar a vulnerabilidade raiz e propor um plano de fortalecimento (hardening) eficaz para a rede, a fim de prevenir futuros incidentes.

---

## O Cenário

A análise foi baseada em um incidente onde uma empresa de multimídia teve seus serviços de rede interrompidos por duas horas. A investigação revelou que a interrupção foi causada por um ataque de negação de serviço que explorou uma vulnerabilidade crítica na infraestrutura de rede da organização:

**Firewall Mal Configurado:** O firewall da empresa não possuía regras para filtrar ou limitar a taxa de pacotes ICMP, permitindo que um agente mal-intencionado sobrecarregasse a rede com um ataque de *ping flood*.

---

## Metodologia de Análise

Para investigar e responder ao cenário, a seguinte metodologia, baseada no NIST CSF, foi aplicada:

* **Análise do Incidente:** Investigação do evento de segurança para determinar o tipo de ataque, o vetor de entrada e o impacto nos serviços da organização.
* **Análise da Causa Raiz (RCA):** Avaliação da configuração da rede para identificar a falha de segurança específica (o firewall mal configurado) que permitiu o sucesso do ataque.
* **Aplicação do Framework NIST:** Utilização das cinco funções do NIST Cybersecurity Framework (Identificar, Proteger, Detectar, Responder e Recuperar) para estruturar a análise e as recomendações de melhoria.
* **Documentação Técnica:** Consolidação de todos os achados e recomendações em um Relatório de Incidente e Plano de Fortalecimento formal.

---

## Relatório do Incidente e Plano de Fortalecimento (PDF)

O relatório completo, detalhando a análise do incidente, a aplicação do framework NIST e as justificativas técnicas para cada recomendação, pode ser encontrado no link abaixo.

* 📄 **[Relatório de Incidente - Versão em Português (PDF)](https://github.com/cleyandson/ddos-incident-analysis-nist/blob/da28bdfda99de9a8d2da51ee9aee02d992fc4e7d/Documents/%5BPT-BR%5D%20Incident%20report%20analysis.pdf)**

---

## Recomendações de Fortalecimento (Hardening)

Com base na análise da causa raiz, as seguintes ações de remediação foram recomendadas para mitigar os riscos identificados:

* **Implementação de Regras de Firewall (Rate Limiting):** Configurar o firewall para limitar a taxa de pacotes ICMP recebidos. Essa medida é a primeira linha de defesa e previne diretamente que a rede seja sobrecarregada pelo mesmo tipo de ataque.
* **Habilitação da Verificação de IP de Origem:** Implementar a verificação de IP de origem (anti-spoofing) no firewall para bloquear pacotes com endereços de IP falsificados, uma tática comum em ataques DDoS.
* **Implantação de IDS/IPS:** Adicionar um Sistema de Detecção e Prevenção de Intrusão (IDS/IPS) para inspecionar o tráfego ativamente e bloquear pacotes com base em assinaturas de ameaças conhecidas ou comportamento suspeito.
* **Monitoramento Contínuo da Rede:** Implementar software de monitoramento de rede para estabelecer uma linha de base (baseline) do tráfego normal e gerar alertas automáticos sobre anomalias, aumentando a velocidade e a eficiência da detecção.

---

## Habilidades Demonstradas

Este projeto destaca as seguintes habilidades essenciais em cibersegurança:

-   ✅ **Análise de Incidentes de Segurança**
-   ✅ **Aplicação do Framework NIST CSF**
-   ✅ **Fortalecimento de Redes (Network Hardening)**
-   ✅ **Análise de Causa Raiz (RCA)**
-   ✅ **Elaboração de Relatórios Técnicos**
-   ✅ **Recomendação de Políticas e Controles de Segurança**

---

## Contato

* **LinkedIn:** [Cleyandson Fragoso](https://www.linkedin.com/in/cleyandson-fragoso/)
* **Email:** cleyandsontech@gmail.com
