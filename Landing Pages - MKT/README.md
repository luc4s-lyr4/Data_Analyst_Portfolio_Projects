<!-- 
Modelo de README para projetos de Análise de Dados
Autor: Lucas Lyra
Instruções: Substitua tudo que estiver entre [colchetes] pelas informações do seu projeto
-->

# 📊 Redução e Otimização da verba de Campanhas de Landing Pages de Marketing.

## 📌 **Objetivo**

Reduzir o orçamento de Landing Pages de origem paga que não estão gerando resultado e realocar parte da verba de Marketing em Landing Pages com origem paga que estão gerando resultado em vendas.  

---

## 📂 **Estrutura do Projeto**
├── data/ # Conjunto de dados brutos e tratados

├── análises/ # Google Sheets

├── PPT/ # Breve resumo com Recomendações para o time de Marketing

├── README.md # Documentação do projeto


---

## 📊 **Fonte de Dados**
- **Origem:** Kaggle: https://www.kaggle.com/datasets/olistbr/marketing-funnel-olist/data
- **Formato:** CSV
- **Descrição:** 8 mil Leads Qualificados de Marketing (MQLs) que solicitaram contato entre 1º de junho de 2017 e 1º de junho de 2018. Eles foram selecionados aleatoriamente a partir do total de MQLs.
- **Dados:**
1. olist_marketing_qualified_leads_dataset: mql_id, first_contact_date, landing_page_id e origin;
2. olist_closed_deals_dataset mql_id, seller_id,	sdr_id,	sr_id, won_date, business_segment, lead_type, lead_behaviour_profile, has_company, has_gtin, average_stock, business_type, declared_product_catalog_size e declared_monthly_revenue.

---

## 🛠 **Recursos utilizados**
- Google Sheets

---

## 📈 **Processo de coleta e análise**
1. **Coleta de Dados**:<br>
Download do csv e importado dentro do Google Sheets.
2. **Limpeza e Tratamento**:<br>
- Criei uma nova base filtrando o campo **origin**, coletando apenas os dados que sejam iguais a "**paid_search**". A nova base chama-se **paid_search MQLs**, totalizando 1.586 linhas.
- Trouxe 4 métricas para minha tabela paid_search MQLs utilizando procv da base Closed_Deals para identificar quais mqls fecharam negócio de paid_search, quantidade de vendas para somar por Landing_page_id no futuro, data da venda e tempo (em meses) do primeiro contato do MQL até o período final de geração de MQLs das campanhas.
3. **Análise Exploratória**:<br>
- Defini a quantidade de vendas como meu fato quantitativo e cruzei com algumas dimensões de tempo, data da venda, tempo LP (em meses), e também, informações de vendas por mês/ano.
- Gerei uma tabela dinâmica para somar as vendas das LPs únicas, totalizando 184 Landing Pages únicas de origem paga e 195 vendas.


## 💡 **Principais Insights**
- Das 184 Landing Pages, apenas 22,9% gerou resultado em vendas;
- O pico das Vendas Ocorreram 
- [Insight 3]

---

## 📌 **Resultados**
- [Link para dashboard ou relatório final]  
- Capturas de tela:
  
![Exemplo de gráfico](link_da_imagem)

---

📄 Licença
Este projeto está sob a licença MIT.

✨ Autor
Lucas Lyra
📧 Email: [seu-email@example.com]
🔗 LinkedIn | Portfólio
