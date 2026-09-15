# Análise da Rotatividade de Colaboradores

## Visão Geral do Projeto

Uma análise orientada a dados para compreender os padrões de saída de colaboradores e identificar factores-chave que impulsionam a rotatividade voluntária.

**Dataset:** 1.470 colaboradores | 35 variáveis | Dados de Departamento de RH

**Objectivo:** Identificar insights acionáveis para reduzir a rotatividade voluntária de 16,1% para níveis de benchmarking industrial.

---

## Descobertas Principais

### Descoberta: Impacto de Horas Extras
- **Colaboradores com horas extras têm 3x maior rotatividade** (30,5% vs 10,4%)
- Departamentos mais afectados: Investigação, Vendas, RH
- **Recomendação:** Implementar limites rigorosos de horas extras e revisão de compensação

### Disparidade Salarial
- **Colaboradores que saem ganham 29,4% menos** que os que ficam
- Cargos entry-level particularmente vulneráveis (Sales Representatives, Lab Technicians)
- **Recomendação:** Benchmarking salarial para funções de alto risco

### Instabilidade de Carreira Inicial
- **35% da rotatividade ocorre nos primeiros 2 anos** na empresa
- Colaboradores jovens (20-25) mostram 35,8% de taxa de rotatividade
- Limite crítico de estagnação de carreira: 2,2 anos na mesma função
- **Recomendação:** Programas de progressão de carreira + mentoria

---

## Estrutura da Análise

1. **Avaliação da Qualidade dos Dados**
   - Verificação de valores em falta
   - Validação de tipos de dados
   - Estatísticas descritivas

2. **Análise de Remuneração**
   - Comparação de salários por status de saída
   - Distribuição salarial por cargo
   - Análise de disparidades

3. **Impacto de Horas Extras**
   - Correlação de horas extras com rotatividade
   - Análise por departamento
   - Comparação de rendimentos

4. **Progressão de Carreira**
   - Análise de tempo de permanência
   - Frequência de promoções
   - Identificação de estagnação profissional

5. **Perfil Demográfico**
   - Análise de grupos etários
   - Padrões de estado civil
   - Distribuição por género

6. **Análise de Correlações**
   - Correlação de variáveis numéricas
   - Visualização de relações

---

## Recomendações

### Acções Imediatas (0-3 meses)
Estabelecer limites de horas extras (máximo 10-15% mensalmente)  
Implementar revisão obrigatória de compensação de horas extras  
Identificar indivíduos de alto risco para contacto de retenção

### Curto Prazo (3-6 meses)
Conduzir benchmarking salarial para funções com >20% rotatividade  
Estabelecer trajectórias claras de progressão de carreira  
Desenvolver estratégias de retenção específicas por cargo

### Longo Prazo (6-12 meses)
Lançar programas de mentoria para colaboradores em fase inicial  
Implementar ciclos de promoção regulares (a cada 2,0-2,5 anos)  
Criar caminhos de desenvolvimento especializados para funções de risco elevado

---

## Detalhes Técnicos

**Ferramentas Utilizadas:**
- Python 3.8+
- pandas (manipulação de dados)
- matplotlib & seaborn (visualização)
- numpy (cálculos)

**Métricas Calculadas:**
- Taxa de Rotatividade: (Saídas / Total) × 100
- Disparidade Salarial: ((Retidos Salário - Saídas Salário) / Retidos Salário) × 100
- Multiplicador de Horas Extras: Taxa Rotatividade Com Horas Extras / Taxa Sem Horas Extras

---

## Como Usar Este Notebook

1. **Instalar dependências:**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

2. **Garantir disponibilidade de ficheiro de dados:**
   - Colocar `Employee_Attrition.csv` no mesmo directório

3. **Executar o notebook:**
   - Abrir em Jupyter Notebook ou JupyterLab
   - Executar células sequencialmente (de cima para baixo)

4. **Interpretar visualizações:**
   - Gráficos de pizza: composição
   - Gráficos de barras: comparação entre grupos
   - Histogramas: distribuições
   - Heatmaps: correlações entre variáveis

---

## Dicionário de Dados (Variáveis Principais)

| Variável | Descrição | Tipo |
|----------|-----------|------|
| Attrition | Colaborador deixou empresa (Yes/No) | Binária |
| MonthlyIncome | Salário mensal | Numérica (USD) |
| OverTime | Trabalha horas extras (Yes/No) | Binária |
| YearsAtCompany | Tempo de permanência | Numérica (anos) |
| YearsInCurrentRole | Tempo no cargo actual | Numérica (anos) |
| YearsSinceLastPromotion | Tempo desde última promoção | Numérica (anos) |
| Age | Idade do colaborador | Numérica (anos) |
| JobRole | Título do cargo | Categórica |
| Department | Departamento | Categórica |
| JobLevel | Nível de senioridade | Numérica (1-5) |

### Termos Técnicos (Referência em Inglês)

| Termo PT | Termo EN | Significado |
|----------|----------|-------------|
| Taxa de Rotatividade | Attrition Rate | Percentagem de saídas |
| Horas Extras | Overtime | Trabalho adicional |
| Saídas | Attrited | Colaboradores que deixaram |
| Retidos | Retained | Colaboradores que ficaram |
| Disparidade | Gap | Diferença |
| Benchmarking | Benchmarking | Comparação com padrões |

---

## Limitações e Ressalvas

- Análise é **transversal** (foto num momento, não longitudinal)
- Não considera **factores externos do mercado laboral** (concorrência, economia)
- Correlação não implica causalidade (é necessária investigação adicional)
- **Recomendação:** Complementar com entrevistas de saída de colaboradores

---

## Notas Finais

Este projecto demonstra:
✓ Capacidade de análise exploratória de dados (EDA)  
✓ Manipulação de dados com Python (pandas)  
✓ Visualização profissional (matplotlib, seaborn)  
✓ Documentação técnica clara  
✓ Pensamento crítico orientado a negócio  

---

## Autor

**Manuela Sales**  
Analista de Dados Júnior | Bootcamp Bytes4Future  
[LinkedIn](www.linkedin.com/in/manuela-sales)

## Notas de Autoria

Projeto de bootcamp desenvolvido em grupo. 
Esta versão documenta minha contribuição principal à análise e implementação técnica.

## Dúvidas?

Para questões sobre a análise, interpretação ou extensões do projecto, consultar as secções detalhadas do notebook com comentários e explicações em Markdown.
