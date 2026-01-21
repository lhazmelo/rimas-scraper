# 🌊 RIMAS Web Scraper & Hydro Analysis
Automação desenvolvida em Python para extração e análise de dados hidrogeológicos do sistema **RIMAS** (Rede Integrada de Monitoramento de Águas Subterrâneas) do Serviço Geológico do Brasil (SGB).

## 🎯 Objetivo
Facilitar a aquisição de séries históricas de nível d'água em poços de monitoramento, automatizando o download de arquivos CSV e calculando métricas fundamentais para estudos de hidrogeologia no aquífero Urucuia.

## 🚀 Funcionalidades
- **Web Scraping Robusto:** Utiliza `Selenium` para navegar na interface dinâmica do RIMAS, lidando com tabelas, iframes e botões ocultos.
- **Geoprocessamento de Texto:** Converte coordenadas brutas (GGMMSS) e metadados de localização diretamente do HTML.
- **Cálculo Automático:** Processa os dados brutos com `Pandas` para gerar:
  - **Variação Total:** Diferença entre o nível final e inicial (Rebaixamento ou Recuperação).
  - **Taxa Anual:** Velocidade de variação do nível estático (m/ano).
- **Output:** Gera um relatório consolidado em Excel (`.xlsx`) pronto para interpretação.

## 🛠️ Tecnologias Utilizadas
- **Python 3.13.7**
- **Selenium WebDriver:** Automação de navegador.
- **Pandas:** Manipulação e limpeza de dados (DataFrames).
- **OpenPyXL:** Exportação para Excel.

## 📦 Como rodar este projeto

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/lhazmelo/rimas-scraper.git](https://github.com/lhazmelo/rimas-scraper.git)
   cd rimas-scraper
