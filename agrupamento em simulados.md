# Prompt para agrupar questões de simulados
## Seu Prompt Otimizado (Passo 1)

Copie e cole este prompt no chat do seu Notebook após carregar o arquivo com as questões:

```
# ROLE: Especialista em Ciência de Dados Pedagógicos e Auditoria de Concursos
 
# CONTEXTO DE ANÁLISE
Você está analisando um banco de dados de questões para um concurso de alto nível (Analista/Auditor). Sua missão é realizar um "Data Mining" pedagógico para identificar a densidade de cobrança e a originalidade dos itens, utilizando ESTRITAMENTE os documentos fornecidos na fonte: [NOME DA FONTE].
 
# TAREFA 1: AGRUPAMENTO TAXONÔMICO
Organize todas as questões por Assunto Principal e Subtema Específico.
* Exemplo: Direito Constitucional (Assunto) -> Remédios Constitucionais: Habeas Data (Subtema).
 
# TAREFA 2: AUDITORIA DE INCIDÊNCIA E SIMILARIDADE
Para cada subtema, classifique os IDs das questões nas seguintes categorias técnicas:
1. IDÊNTICAS: Questões com enunciado e alternativas rigorosamente iguais.
2. SIMILARES (NÚCLEO COMUM): Questões que, embora com redações diferentes, exigem o conhecimento do mesmo artigo de lei, mesma norma contábil (CPC/MCASP), fórmula ou conceito técnico.
3. RARAS (BAIXA INCIDÊNCIA): Temas que aparecem de forma isolada (ex: uma nota de rodapé ou exceção da exceção).
4. ÚNICAS: Questões sem correspondência direta, que cobram algo que difere totalmente dos demais agrupamentos.
 
# SAÍDA ESPERADA (RELATÓRIO ESTRUTURADO)
Apresente a análise seguindo rigorosamente esta estrutura para cada grupo:
 
---
### TEMA: [NOME DO TEMA]
**Subtema:** [Nome do Subtema]
* **Volume:** [X] questões identificadas.
* **IDs das Questões:** [Listar IDs numéricos conforme constam na fonte].
* **Padrão de Repetição:** [Alta / Média / Baixa Incidência].
* **Análise de Similaridade:** "As questões [IDs] orbitam o núcleo comum: [Citar brevemente a lei/norma/conceito]".
* **Destaque de Raridade:** [Identificar se há questões 'ponto fora da curva' ou inéditas].
---
 
# RESTRIÇÕES DE INTEGRIDADE E EXECUÇÃO
* FIDELIDADE TOTAL: Utilize apenas IDs e textos presentes nos documentos carregados. Não utilize conhecimento externo ou invente questões.
* PROCESSAMENTO EXAUSTIVO: Analise o bloco completo (até 200 questões). Não interrompa a análise antes de mapear todos os IDs disponíveis na fonte.
* FOCO EM AUDITORIA: Diferencie nuances técnicas para agrupar as 'Similares'.
```

Sugestão adicional: pegue a resposta da IA e clique em "Salvar nas observações". Isso vai criar uma nota, depois clique em "Transformar em fonte" para que tenha os dados do seu simulado como fonte. 

---

### Seu Prompt Otimizado (Passo 2)

Use este prompt após a IA ter entregue o relatório do Passo 1:


```
# ROLE: Designer Instrucional e Especialista em Ciência da Aprendizagem
 
# TAREFA
Converter o mapeamento de questões anterior em uma "Matriz de Tópicos de Estudo Atômicos". Sua missão é destilar o ruído das repetições e focar no núcleo de conhecimento necessário para acertar as questões.
 
# DIRETRIZES DE ENGENHARIA PEDAGÓGICA
 
1. FUSÃO E SÍNTESE: Para cada agrupamento de questões "Similares" ou "Idênticas", extraia o núcleo comum. Não repita o tema; crie uma única unidade de conhecimento que resolva todas as questões daquele grupo.
 
2. ATOMICIDADE (Carga Cognitiva): Se um tema for complexo (ex: Tópico complexo), fragmente-o em tópicos menores (ex: 1. sub-tópico; 2. sub-tópico; 3. sub-tópico). Cada tópico deve ser uma "pílula" de informação independente.
 
3. FOCO NO "FATO GERADOR": A descrição do tópico deve focar no que o examinador realmente cobra (o 'pegadinha' recorrente, o prazo específico, a exceção da norma ou a fórmula chave).
 
4. PRIORIZAÇÃO POR DENSIDADE: Ordene a tabela dos tópicos com mais questões (maior incidência) para os de menor incidência.
 
# SAÍDA (TABELA DE TÓPICOS DE ESTUDO ADAPTADOS)
Gere uma tabela com as seguintes colunas:
 
| Nº | Tópico de Estudo (Atômico) | Foco da Cobrança (O que dominar) | Relevância (Baseada no Volume) |
|:---|:---|:---|:---|
| 01 | [Nome do Tópico] | [A regra, lei ou conceito central] | [Alta / Média / Baixa] |
| 02 | [Nome do Tópico] | [A regra, lei ou conceito central] | [Alta / Média / Baixa] |
 
# RESTRIÇÃO
Mantenha a terminologia técnica rigorosa (Direito, Contabilidade, Auditoria). Não generalize termos técnicos.
```

Sugestão adicional: pegue a resposta da IA e clique em "Salvar nas observações". Isso vai criar uma nota, depois clique em "Transformar em fonte" para que tenha a matriz dos tópicos mais importantes do seu simulado como fonte. 
