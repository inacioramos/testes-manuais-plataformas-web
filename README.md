# 🛡️ Portfólio de Testes Manuais de Software

Olá! Este repositório concentra meus projetos práticos de **Quality Assurance (QA)**, focados em testes manuais, validação de critérios de aceite, análise de interface (UI/UX) e comportamento de formulários em plataformas web de grande escala.

---

## 💻 Cenários de Teste Executados

### 1. Teste Funcional de Busca e Filtros (Mercado Livre)
* **Objetivo:** Validar a resiliência do sistema de buscas e a precisão dos filtros combinados (Marca + Faixa de Preço) e ordenação.
* **O que foi testado:** Fluxo positivo de busca por "notebook", filtros por marca (Acer), filtros por preço (R$ 4.000 a R$ 5.000) e ordenação por menor preço.
* **Resultados:** Identificado comportamento inesperado (Falha) ao buscar termos inexistentes, onde o sistema retornou produtos aleatórios em vez de "nenhum produto encontrado".

### 2. Teste de Interface e Consistência Visual (Amazon)
* **Objetivo:** Garantir a integridade visual, responsividade do header, alinhamento de menus e comportamento de elementos em hover.
* **O que foi testado:** Alinhamento horizontal do menu superior, contraste do texto para acessibilidade, tempo de carregamento de banners/carrosséis (validado abaixo de 2 segundos) e o comportamento do menu *dropdown* "Contas e Listas".

### 3. Teste de Validação de Formulário e Segurança (LinkedIn)
* **Objetivo:** Avaliar o comportamento do formulário de cadastro sob entradas inválidas (Boundary Value Analysis).
* **O que foi testado:** Envio de campos vazios, formatos inválidos de e-mail (sem @, sem domínio, apenas números) e força/composição de senhas.
* **Destaque Técnico (Análise Crítica):** * Identifiquei falhas severas na validação de dados de entrada do formulário. O sistema permitiu o avanço no cadastro utilizando formatos inválidos de e-mail (como apenas números) e aceitou senhas sem a composição mínima exigida pelas regras de negócio (senhas compostas apenas por letras ou apenas por números sem caracteres especiais).

---

## 📊 Relatório de Métricas (Test Report)
Durante as rodadas de testes, consolidei os seguintes indicadores de qualidade do software:

| Métrica | Build Atual | Build Anterior | Status |
| :--- | :---: | :---: | :---: |
| **Total de Casos de Teste (TCs)** | 13 | 9 | ⇑ |
| **Casos Passados** | 6 | 9 | ⇓ |
| **Casos Falhados** | 4 | 0 | ⇑ |
| **Casos Bloqueados** | 3 | 0 | ⇑ |

### Distribuição de Defeitos (Build Atual)
* **Severidade Alta:** 4 defeitos.
* **Tipo de Defeito:** 4 Funcionais / 3 de UI-UX.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Ambiente de Testes:** Windows 11 | Google Chrome (v145.0)
* **Documentação:** Modelagem de Casos de Teste e Reporte de Métricas via Planilhas/CSV.
* **Técnicas Aplicadas:** Teste de Caixa Preta, Análise de Valor Limite, Partição de Equivalência, Teste Exploratório.
