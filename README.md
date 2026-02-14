🎮 Xbox Game Pass – Sales Dashboard (Excel)


📌 Sobre o Projeto

Este projeto consiste no desenvolvimento de um Dashboard de Vendas de Assinaturas do Xbox Game Pass, construído no Microsoft Excel, com foco em:

📊 Análise de faturamento

💰 Receita por plano

🎮 Receita com Season Pass

🔄 Análise de renovação automática

📈 Suporte à tomada de decisão estratégica


O dashboard foi estruturado seguindo boas práticas de organização em camadas:

Dados → Tratamento → Visualização


🗂 Estrutura da Planilha

O arquivo está dividido nas seguintes abas:

📁 Assets

Área de apoio visual contendo:

Paleta de cores

Identidade visual

Elementos gráficos utilizados no dashboard

📁 Bases

Base de dados principal do projeto.

Principais Colunas:
Campo	Descrição
Subscriber ID	Identificador do assinante
Plan	Plano contratado (Ultimate, Core, Standard)
Subscription Type	Monthly, Quarterly ou Annual
Subscription Price	Valor do plano
EA Play Season Pass	Indicador de compra adicional
Minecraft Season Pass	Indicador de compra adicional
Coupon Value	Valor de desconto aplicado
Total Value	Valor final pago
Auto Renewal	Indica renovação automática

⚠️ Esta é a única aba que deve ser editada para atualização do dashboard.


📁 Cálculos

Camada intermediária responsável por:

Consolidação de métricas

Fórmulas agregadas

Cálculos financeiros

Preparação de dados para o Dashboard

Principais Funções Utilizadas:

SOMASE()

SOMASES()

CONT.SE()

CONT.SES()

PROCV() ou PROCX()

Tabelas Dinâmicas

Cálculo de percentuais

📁 Planos

Base auxiliar com:

Estrutura de planos

Validação de dados

Apoio para buscas e cruzamentos

📁 Dashboard

Interface visual e executiva do projeto.

Principais Indicadores (KPIs):

💰 Receita Total

👥 Total de Assinantes

🎮 Receita com Season Pass

📊 Receita por Plano

🔄 Distribuição de Auto Renewal

📊 Métricas do Projeto
Receita Total
=SOMA(Total Value)

Ticket Médio
=Receita Total / Total de Assinantes

Receita por Plano
=SOMASE(Plan; "Ultimate"; Total Value)

Receita com Passes
=SOMA(Receita Total Pass)

▶️ Como Utilizar a Planilha
1️⃣ Atualizar Base de Dados

Inserir novos registros na aba Bases.

Não alterar nomes das colunas.

2️⃣ Atualizar Dashboard
Dados → Atualizar Tudo

ou botão direito nas Tabelas Dinâmicas → Atualizar

3️⃣ Utilizar Segmentações (se aplicável)

Permite filtrar por:

Plano

Tipo de assinatura

Auto Renewal

Período

🚀 Melhorias Futuras

 Implementar análise de crescimento mensal

 Adicionar meta vs realizado

 Automatizar dados com Power Query

 Implementar análise de ticket médio por plano

 Criar comparativo por período

 Avaliação de impacto de descontos


🏷 Tecnologias Utilizadas

Microsoft Excel

Fórmulas condicionais

Tabelas Dinâmicas

Segmentações de Dados

Design orientado a KPIs


📌 Conclusão

Este projeto entrega uma visão estratégica das vendas de assinaturas do Xbox Game Pass, permitindo:

Identificação de planos mais rentáveis

Análise de comportamento de renovação

Suporte à tomada de decisão
