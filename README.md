# Web Scraping de Dados da Receita Federal

![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/-BeautifulSoup4-3776AB?style=flat-square&logo=python&logoColor=white)
![Colab](https://img.shields.io/badge/-Google%20Colab-F9AB00?style=flat-square&logo=google-colab&logoColor=white)

Projeto de web scraping para coleta automatizada de dados de empresas disponibilizados pela Receita Federal do Brasil.

## Resultados Obtidos

- 📊 Dados estruturados de CNPJs atualizados
- 📂 Arquivos organizados por período (formato AAAA-MM)
- ⚡ Processo de coleta automatizado e eficiente
- 🕒 Redução de tempo na obtenção dos dados em comparação com métodos manuais

## 💼 Aplicações Práticas

Os dados coletados podem ser utilizados para:

- 🔍 Análise de mercado e competidores
- 📈 Business Intelligence
- 🕵️♂️ Verificação de informações empresariais
- 📑 Integração com sistemas de CRM e ERP
- 🧠 Projetos de Machine Learning e Data Science

## 🎯 Objetivo

Automatizar a coleta de dados corporativos do Banco de Dados Público da Receita Federal, organizados cronologicamente no formato `AAAA-MM` (ano com 4 dígitos e mês com 2 dígitos).

## 🔗 Fonte de Dados

Os dados são obtidos diretamente do portal oficial da Receita Federal:

[Banco de Dados da Receita Federal](https://arquivos.receitafederal.gov.br/cnpj/)

## ⚙️ Funcionalidades Principais

- ✅ Download automatizado de arquivos diretamente da fonte oficial
- 📅 Organização inteligente dos dados por período (formato AAAA-MM)
- ☁️ Execução nativa no Google Colab (sem necessidade de ambiente local)
- ⏳ Sistema de manutenção de conexão ativa para processos longos

## 🚀 Como Executar no Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1X_c6IHV9lnXNM81C339Ia1o0onaaBf7s?usp=sharing)

1. Acesse o notebook via link acima
2. Execute as células sequencialmente:
   - Instalação automática de dependências
   - Configuração do ambiente
   - Processo de scraping e download
3. Os arquivos serão salvos no ambiente do Colab e podem ser:
   - Exportados para Google Drive
   - Baixados manualmente

## 📦 Dependências

| Biblioteca | Versão | Finalidade |
|------------|--------|------------|
| BeautifulSoup4 | 4.x | Parsing de HTML/XML |
| requests | 2.x | Requisições HTTP |

Todas as dependências são instaladas automaticamente durante a execução inicial.

## ⚠️ Manutenção de Conexão

Para evitar desconexões em processos longos:

```python
from google.colab import output
output.eval_js('google.colab.kernel.proxyPort(5000)')
