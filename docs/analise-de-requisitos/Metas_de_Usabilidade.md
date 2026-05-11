# Metas de Usabilidade

## Introdução

Este artefato tem como propósito definir as metas de usabilidade que estabelecem quais fatores de qualidade de uso devem ser priorizados no projeto, além de como a avaliação ocorrerá durante o processo de design quais faixas de valores são aceitáveis ou inaceitáveis. As mestas de usabilidades tratadas
nesse documento são as definidas pelos pesquisador Jacob Nielsen, sendo fundamentais para o design de sistemas computacionais  mais intuitivos e
agradáveis para os usuários dentro da nossa aplicação.

## Definição das Metas de Usabilidade

- **Eficácia:** Referente á qualidade do produto, se ele é bom em fazer o que se espera que faça.

- **Eficiência:** Referente a como o sistema ajuda o usuário a realizar determinadas atividades com a menor quantidade de etapas possível.

- **Segurança:** Referente à proteção do usuário de condições perigosas e situações indesejáveis, prevenindo erros graves e, casso ocorram, oferecendo
maneiras de recuperar ou desfazer ações.

- **Utilidade:** Referente às medidas e funcionalidades concedidas ao usuário para a realização da atividade de interesse.

- **Aprendizagem:** Referente à facilidade de aprendizado do sistema, para que o usuário consiga aprender a utilizá-lo rapidamente e se torne competente
na realização das tarefas.

- **Memorização:** Referente à capacidade do usuário de lembrar como utilizar o sistema após já ter aprendido, especialmente importante em sistemas
acessados com pouca frequência.

## Metas a serem almejadas pelo nosso projeto

Com a intenção de definir as metas almejadas no projeto, analisamos o site de matrículas do Distrito Federal e identificamos as mets definidas por
Nielsen mais críticas, decidindo trabalhar prioritariamente sobre elas. A seguir, analisamos as metas de usabilidade do [Sistema de Matrículas do DF](https://www.educacao.df.gov.br/) por meio de perguntas direcionadas a cada meta:

### **Eficácia**

- **Pergunta:** O sistema cumpre seu propósito principal de permitir que o responsável legal realize a matrícula do estudante de forma completa?

- **Meta Apliacada:** Sem meta. O sistema de matrículas em sua função central de registrar solicitações de matrículas, cumpre seu objetivo principal. No
entanto, há falhas pontuais como ausência de confirmação clara ao final do processo.

--- 

### **Eficiência**

- **Pergunta:** O sistema permite ao usuário concluir a matrícula com o menor número de etapas possível? O fluxo é direto e sem redundâncias?

- **Meta aplicada:** O sistema apresenta problemas de eficiência, pois exige que o usuário navegue por múltiplas páginas sem indicação clara de
progresso, além de solicitar informações repetidas em etapas distintas do processo. Dessa forma, obtivemos como meta redundâncias e exibindo um indicador
de progresso vísivel duranre todo o processo, conforme ilustrado na Figura 1.

> **Figura 1** - Capturar a tela do fluxo atual mostrando a ausência de indicador de progresso entre às páginas e a navegação confusa entre páginas.

---

### **Segurança**

- **Pergunta:** O sistema permite ao usuário reverter ações indesejadas? Há confirmação antes de ações críticas como cancelamento de matrícula?

- **Meta aplicada:** O sistema não oferece mensagens de confirmação antes de ações irreversíveis, como cancelamento de uma solicitação de matrícula, nem
permite que o usuário retorne a etapas anteriores sem perder os dados já preenchidos. Assim, obtivemos como meta implementar diálogos de confirmação em
ações críticas e permitir navegação entre etapas sem perda de dados, conformer ilustrado na Figura 2.

> **Figura 2** - Aqui deve tirar um print da tela onde o usuário perde dados ao clicar em "voltar" ou pode ser também quando não há confirmação antes de uma ação crítica.

### **Utilidade**

- **Pergunta:** O sistema oferece o conjunto adequado de funcionalidades para que o usuário realize sua matrícula? O usuário recebe feedback visual do
que está acontecendo?

- **Meta aplicada:** Sem meta. O sistema oferece as funcionalidades básicas necessárias para a realização da matrícula, como seleção de escola, turno e
etapa de ensino, atendendo à meta de utilidade.

---

### **Aprendizagem**

- **Pergunta:** O usuário consegue aprender a usar o sistema com facilidade na primeira utilização, sem necessidade de ajuda externa?

- **Meta aplicada:** O sistema apresenta dificuldades de aprendizagem, pois sua interface inicial é carregada de informações institucionais que desviam o
usuário do fluxo principal de matrícula. Rótulos de campo e botões são poucos descritiveis, exigindo tentativa e erro para compreensão. Dessa forma,
obtivemos como meta simplificar a interface inicial, destacar claramente o ponto de entrada do fluxo de mátricula e tornar os rótulos mais descritivos e
intuitivos, comforme ilustrado na Figura 3.

> **Figura 3** - Capturar a tela inicial do sistema de matrículas mostrando o excesso de informações.

### **Memorização**

- **Pergunta:** O sistema oferece suporte suficiente para que um usuário que o acessa raramente (uma vez por ano, no período de matrículas) consiga
utilizá-lo sem dificuldades?

- **Meta aplicada:** O sistema não oferece suporte de interface para auxiliar usuários que o acessam com pouca frequência, como tutoriais ou indicações
contextuais sobre o que fazer em cada etapa. Considerando que a matrícula ocorre anualmente, a memorização é especialmente crítica. Dessa forma,
obtivemos como meta adicionar textos de ajuda contextuais em cada etapa do formulário e disponibilizar um FAQ acessível durante o processo, conforme
ilustrado na Figura 4.

> **Figura 4** -  Capturar a tela de algum campo do formulário que não possui qualquer instrução de auxílio.

---

## Conclusão

Portanto, neste artefato foram abordadas as definições das metas de usabilidade, avaliadas por meio de perguntas que direcionaram a análise do sistema de
matrículas do DF. Após a análise de todas as metas definidas por Nielsen, ficou decidiso que as metas mais críticas dentro do sistema e que serão
almejadas no escopo do projeto são:

- **Eficiência:** Reorganizar o fluxo em etapas sequenciais com indicador de progresso visível.
- **Segurança:** Implementar confirmações em ações críticas e preservar dados ao navegar entre etapas.
- **Aprendizagem:** Simplificar a interface inicial e tornar rótulos mais intuitivos.
- **Memorização:** Adicionar textos de ajuda contextuais e FAQ acessível durante o processo.

## Bibliografia

> [1] NIELSEN, Jacob. *Designing Web Usability: The Practice of Simplicity.* Peachpit Press, 1999.
>
> [2] BARBOSA, S. D. J.; SILVA, B. S. da; et al. *Interação Humano-Computador e Experiência 
> do Usuário.* 2021.
>
> [3] FOURNIER, Diana. As 6 metas de Usabilidade. Medium, 2016. Disponível em: 
> https://medium.com/vivareal-ux-chapter/as-6-metas-de-usabilidade-9491442fd56a
>
> [4] DISTRITO FEDERAL. Sistema de Matrículas. Disponível em: 
> https://www.matricula.se.df.gov.br/

## Histórico de Versões

Versão | Data | Descrição | Autor(es) | Revisor(es) |
|---|---|---|---|---|
| `1.0` | 11/05/2026 | Criação da página Metas de Usabilidade | [Joao Guilherme](https://github.com/JoaoGSantana10) | |
