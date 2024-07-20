
## Autenticação Facial para Prevenção de Fraudes

**Introdução**

O setor de fraudes da Quantumn Finance identificou um problema recorrente de clientes que contestam a contratação de serviços específicos, como crédito pessoal, mesmo após a realização dos protocolos de segurança da senha. Apesar da autenticação por senha, o banco arca com reembolsos e medidas de contenção para evitar processos judiciais, pois os clientes alegam terem sido vítimas de invasão por hackers ou outras atividades fraudulentas.

**Proposta**

Para mitigar esse risco e fortalecer a segurança nas transações, propõe-se a implementação de um sistema de autenticação facial complementar à senha, utilizando a plataforma **Amazon Rekognition** da AWS.


Neste projeto, focaremos na funcionalidade de **Classificação de Texto** para categorizar os assuntos dos atendimentos.

Participantes do projeto:

Grupo:

| Nome    | RM            | Turma |
| :----------------------- | :------------- | :-----: |
| Igor Mazzeto             | RM 352368      | 5DTSR |
| Gildo Moraes             | RM 352486      | 5DTSR |
| Luiz Henrique             | RM 352631      | 5DTSR |

**Amazon Rekognition**

O Amazon Rekognition é um serviço de **visão computacional e aprendizado de máquina** baseado em nuvem que oferece diversas funcionalidades para análise de imagens e vídeos, incluindo:

* **Detecção de rostos:** Localiza e identifica rostos em imagens e vídeos.
* **Reconhecimento facial:** Compara rostos em imagens e vídeos com rostos em um banco de dados para verificar a identidade de uma pessoa.
* **Detecção de emoções:** Analisa as emoções presentes em rostos em imagens e vídeos.
* **Detecção de atividades:** Reconhece atividades como comer, beber e falar em imagens e vídeos.
* **Análise de cenas:** Identifica e classifica objetos, cenas e atividades em imagens e vídeos.

**Solução Proposta**

O sistema de autenticação facial funcionará da seguinte maneira:

1. **Cadastro de imagens:** Os clientes cadastrarão suas imagens faciais no banco de dados do sistema durante a abertura de conta ou solicitação de serviços.
2. **Autenticação por senha e rosto:** Ao realizar transações que exigem alto nível de segurança, como solicitação de crédito, o cliente será solicitado a se autenticar com sua senha e realizar uma verificação facial.
3. **Validação facial:** O Amazon Rekognition utilizará as funcionalidades de detecção e reconhecimento facial para comparar a imagem capturada em tempo real com a imagem cadastrada do cliente.
4. **Detecção de vivacidade:** Para garantir que o cliente esteja realmente presente e não utilizando uma foto estática, a detecção de vivacidade verificará se a imagem capturada apresenta características de um rosto real, como piscar ou mover a cabeça.
5. **Autenticação bem-sucedida:** Se a autenticação facial for bem-sucedida, a transação será autorizada.
6. **Autenticação malsucedida:** Se a autenticação facial falhar, o cliente será direcionado para uma esteira de atendimento dedicada, e as imagens da tentativa de autenticação serão encaminhadas para a área de IA para análise e aprimoramento do modelo.

**Benefícios**

A implementação da autenticação facial trará diversos benefícios para o Banco X:

* **Redução de fraudes:** A autenticação facial dificulta a realização de transações fraudulentas por terceiros, pois exige a presença física do cliente.
* **Maior segurança para os clientes:** Os clientes terão mais segurança ao realizar transações, pois a autenticação por dois fatores (senha e rosto) torna mais difícil o acesso não autorizado às suas contas.
* **Diminuição de custos:** A redução de fraudes levará à diminuição de custos com reembolsos e medidas de contenção.
* **Melhoria da experiência do cliente:** A autenticação facial proporcionará uma experiência mais rápida e segura para os clientes, reduzindo filas e tempo de espera.
* **Geração de dados para análise:** As imagens da tentativa de autenticação facial poderão ser utilizadas para aprimorar o modelo de autenticação e identificar padrões de comportamento fraudulento.


A implementação da autenticação facial com o Amazon Rekognition é uma solução eficaz para combater fraudes e aumentar a segurança das transações no Banco X. Além de reduzir custos e melhorar a experiência do cliente, o sistema também gerará dados valiosos para análise e aprimoramento contínuo.






