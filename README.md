# aws-step-functions-lab
 Repositório organizado contendo anotações e insights adquiridos durante a prática
# Conceitos Fundamentais - AWS Step Functions

## O que são Step Functions?
- Serviço da AWS para **orquestrar workflows**.  
- Permite integrar vários serviços da AWS em **fluxos automatizados e visuais**.  
- Usa **Amazon States Language (ASL)** (JSON) para definir a lógica.

---

## Tipos de Estados
1. **Pass** → Passa informações adiante sem executar nada.  
2. **Task** → Executa uma tarefa (ex: chamar Lambda, SQS, DynamoDB).  
3. **Choice** → Define condições lógicas (if/else).  
4. **Wait** → Atraso definido por tempo.  
5. **Parallel** → Executa tarefas em paralelo.  
6. **Map** → Itera sobre listas de itens.  
7. **Fail** → Marca a execução como falha.  
8. **Succeed** → Marca a execução como sucesso.

---

## Tipos de Workflows
- **Standard**  
  - Ideal para processos de longa duração (até 1 ano).  
  - Milhões de execuções.  
- **Express**  
  - Focado em **alta taxa de requisições** e execução rápida.  
  - Mais barato para grande volume de eventos.

---

## Casos de Uso
- Processamento de imagens (S3 + Lambda).  
- Orquestração de ETL (Glue, EMR).  
- Processos de aprovação (DynamoDB + SNS + Lambda).  
- Pipelines de dados ou machine learning.  
