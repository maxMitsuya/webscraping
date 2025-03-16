# Web Scraping de Dados da Receita Federal

Este projeto consiste em uma aplicação de **web scraping** desenvolvida utilizando a biblioteca **Beautiful Soup 4**. Foi criado como parte de um projeto prático realizado durante o curso na **DNC**. O código foi desenvolvido para ser executado diretamente no **Google Colab**, facilitando o acesso e a reprodução.

## Objetivo

O objetivo principal deste projeto é automatizar o processo de coleta de dados sobre empresas disponibilizados pela **Receita Federal**. A aplicação realiza o download dos dados diretamente do Banco de Dados da Receita Federal, organizados por data no formato "ano-mês" (onde o ano é representado por quatro dígitos e o mês por dois dígitos).

## Fonte dos Dados

Os dados utilizados neste projeto são disponibilizados publicamente pela Receita Federal e podem ser acessados através do seguinte link:  
[Banco de Dados da Receita Federal](https://arquivos.receitafederal.gov.br/cnpj/)

Os arquivos estão organizados por data, seguindo o padrão "ano-mês" (exemplo: `2023-10` para outubro de 2023).

## Funcionalidades

- **Automatização do Download**: O script realiza o download automático dos arquivos de dados diretamente do site da Receita Federal.
- **Organização por Data**: Os dados são baixados e organizados de acordo com a data de publicação, facilitando a análise e o processamento posterior.
- **Execução no Google Colab**: O código foi desenvolvido para ser executado diretamente no Google Colab, permitindo que qualquer pessoa possa rodá-lo sem a necessidade de configurar um ambiente local.

## Como Usar no Google Colab

1. Acesse o notebook no Google Colab através do link fornecido: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://colab.research.google.com/drive/1XZtg6Swi6ulJ0Ht4mcURq7tJHBfJ0Bts?usp=sharing](https://colab.research.google.com/drive/1X_c6IHV9lnXNM81C339Ia1o0onaaBf7s?usp=sharing))
2. Certifique-se de que o ambiente do Colab está configurado corretamente (todas as bibliotecas necessárias já estão incluídas no código).
3. Execute as células do notebook na ordem:
   - A primeira célula instala as dependências necessárias.
   - As células seguintes realizam o scraping e o download dos dados.
4. Os arquivos baixados serão salvos no ambiente do Colab e podem ser exportados para o Google Drive ou baixados manualmente.

## Requisitos

O código foi desenvolvido para ser executado no **Google Colab**, portanto, não é necessário instalar nada localmente. As bibliotecas necessárias são instaladas automaticamente no início do notebook. As principais bibliotecas utilizadas são:

- **Beautiful Soup 4** (`bs4`)
- **Requests** (`requests`)

## Código para Manter a Conexão Ativa

Durante a execução no Google Colab, é comum que a sessão seja desconectada após um período de inatividade. Para evitar isso, utilizamos o seguinte código:

```python
from google.colab import output
output.eval_js('google.colab.kernel.proxyPort(5000)')
```

## Contribuição
Contribuições são bem-vindas! Se você tiver sugestões de melhorias ou encontrar algum problema, sinta-se à vontade para abrir uma issue ou enviar um pull request.

