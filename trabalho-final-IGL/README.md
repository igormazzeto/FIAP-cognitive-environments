## Classificador de Assuntos de Atendimento

**Introdução**

Este projeto visa desenvolver um modelo de Machine Learning para classificar automaticamente os assuntos dos atendimentos no canal de chat da QuantumFinance. O objetivo é otimizar o direcionamento dos chamados para as áreas especialistas, aprimorando a experiência do cliente e a eficiência da empresa.

**Serviço Utilizado**

Para a criação do modelo classificador, será utilizado o **Amazon Comprehend**, um serviço de processamento de linguagem natural (NLP) da AWS. O Comprehend oferece diversas funcionalidades, incluindo:

* **Análise de Sentimento:** Determina a polaridade emocional de um texto (positivo, negativo, neutro).
* **Extração de Entidades:** Identifica e classifica entidades nomeadas em um texto (pessoas, lugares, organizações).
* **Detecção de Tópico:** Classifica um texto em um conjunto predefinido de tópicos.
* **Classificação de Texto:** Atribui um rótulo predefinido a um texto com base em seu conteúdo.

Neste projeto, focaremos na funcionalidade de **Classificação de Texto** para categorizar os assuntos dos atendimentos.

Participantes do projeto:

Grupo:

| Nome    | RM            | Turma |
| :----------------------- | :------------- | :-----: |
| Igor Mazzeto             | RM 352368      | 5DTSR |
| Gildo Moraes             | RM 352486      | 5DTSR |
| Luiz Henrique             | RM 352631      | 5DTSR |



**Dados**

O modelo será treinado e validado utilizando o dataset **"tickets_reclamacoes_classificados.csv"**, disponível no seguinte link:

```
https://dados-ml-pln.s3.sa-east-1.amazonaws.com/tickets_reclamacoes_classificados.csv
```

Este dataset contém registros de atendimentos no chat, com o texto da mensagem do cliente e a respectiva categoria do assunto (rótulo).

**Metodologia**

1. **Pré-processamento:** O dataset será pré-processado para remover ruídos, normalizar o texto e converter em um formato adequado para o modelo de Machine Learning.
2. **Treinamento do Modelo:** O modelo de Classificação de Texto do Amazon Comprehend será treinado utilizando o dataset pré-processado.
3. **Validação do Modelo:** O modelo treinado será validado em um conjunto de dados separado (25% do dataset original) para avaliar seu desempenho e garantir que ele não esteja apenas memorizando os dados de treinamento.
4. **Otimização do Modelo:** Caso o modelo não atinja o score desejado na métrica F1 Score (acima de 75%), serão realizadas técnicas de ajuste de hiperparâmetros e otimização de dados para melhorar sua performance.
5. **Implementação:** O modelo final será implementado em uma aplicação que permita a classificação automática dos assuntos dos atendimentos em tempo real.

**Plataforma de Machine Learning**

O desenvolvimento da solução será realizado na plataforma **Amazon Web Services (AWS)**, utilizando os serviços:

* **Amazon Comprehend:** Para treinamento e validação do modelo de Classificação de Texto.
* **Amazon S3:** Para armazenamento do dataset.
* **AWS Lambda:** Para execução da função de classificação automática.
* **Amazon API Gateway:** Para criar uma API que permita a integração com o canal de chat da QuantumFinance.

**Objetivos**

Ao implementar este modelo de classificação de assuntos, a QuantumFinance poderá otimizar o direcionamento dos chamados no canal de atendimento ao cliente, proporcionando uma experiência mais rápida e eficiente para seus clientes. Além disso, a solução poderá gerar insights valiosos sobre os principais temas dos atendimentos, auxiliando na identificação de oportunidades de melhoria nos produtos e serviços da empresa.

Os resultados obtidos com a implementação do modelo de classificação de assuntos utilizando o SDK do Amazon Comprehend serão apresentados em um notebook em Python.



