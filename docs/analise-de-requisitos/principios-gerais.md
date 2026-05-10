## Princípios Gerais do Projeto

## Introdução

Os princípios gerais do projeto constituem uma parte fundamental no desenvolvimento do trabalho como um todo, servindo como guia para a análise e proposta de melhorias na plataforma estudada. Como as funcionalidades escolhidas pelos integrantes ainda não existem na plataforma, serão descritos o objetivo de cada princípio e uma violação identificada no site atual, a fim de servir de guia nas próximas etapas do projeto — ilustrando tanto o que não deve ser feito quanto o que deveria ser implementado. Os princípios e diretrizes utilizados no presente projeto estão, com base em Barbosa e Silva (2021), ligados aos seguintes tópicos [1]:

## Princípios

### Simplicidade das Estruturas das Tarefas

Esse princípio visa simplificar a estrutura das tarefas disponíveis ao usuário, reduzindo informações desnecessárias e destacando apenas o que é pertinente para a conclusão de cada etapa. Dessa forma, facilita-se o aprendizado e torna-se a navegação mais fluida e intuitiva.

**Violação identificada no site da Educação DF:**
O menu de navegação principal do site apresenta estrutura excessivamente extensa e com múltiplos níveis de profundidade, contendo submenus dentro de submenus que dificultam a localização de serviços simples. A seção "Carta de Serviços", por exemplo, está acessível apenas por meio do caminho **Serviços > Carta de Serviços**, que não é intuitivo para um cidadão que acessa o site pela primeira vez em busca de informações sobre matrícula ou remanejamento escolar. Além disso, a página da Carta de Serviços exibe uma lista de dez categorias sem qualquer descrição ou hierarquia visual que oriente o usuário sobre qual delas corresponde à sua necessidade.

---

### Consistência e Padronização

A padronização, quando acordada entre os responsáveis pelo sistema, permite manter a consistência visual e funcional do site, evitando que o usuário se sinta desorientado ao navegar entre páginas e funcionalidades distintas.

**Violação identificada no site da Educação DF:**
E vários locais o site possui sessões de informações com botões de navegação entre uma categoria da informação e outra, a cor não é padronizada, em alguns é azul, outras verde, outras roxa. Isto dificulta o entendimento do site, trazendo mais informação do que o necessário para o usuário processar.

---

### Promovendo a Eficiência do Usuário

Tognazzini (2003) recomenda considerar sempre a eficiência do usuário em primeiro lugar, e não a do computador. Processamentos demorados não devem prender a interação, mas permitir que os usuários continuem seu trabalho com outras partes do sistema. Além disso, o sistema deve proteger o trabalho dos usuários — eles nunca devem perder dados por erros próprios, falhas de rede ou qualquer outra razão. Para usuários frequentes, Nielsen (1993) e Shneiderman (1998) recomendam fornecer atalhos e aceleradores que reduzam o número de interações e acelerem o ritmo de uso [1].

**Violação identificada no site da Educação DF:**
O site não oferece nenhum mecanismo de aceleração ou atalho para usuários recorrentes, como responsáveis que acessam o sistema anualmente para solicitar remanejamento escolar. Não há área de acesso rápido por perfil de usuário, salvamento de dados previamente preenchidos, nem qualquer forma de o sistema reconhecer que o usuário já passou por aquele fluxo anteriormente. Cada acesso exige que o cidadão repercorra todos os níveis de navegação do zero, sem atalhos ou memória de sessão que otimizem o processo.

---

### Projeto para Erros

Recomenda-se projetar o sistema assumindo que qualquer erro potencial poderá ser cometido pelo usuário. O sistema deve ajudá-lo a se recuperar de um erro, informando o que ocorreu, as consequências e como reverter os resultados indesejados [1].

**Violação identificada no site da Educação DF:**
A página da Carta de Serviços não apresenta nenhum mecanismo de orientação preventiva ao usuário antes de iniciar um processo. As categorias listadas — como "Matrícula", "Vida escolar" e "Benefício educacional" — não oferecem qualquer descrição prévia sobre o que cada seção contém, nem alertam sobre prazos ou documentos necessários antes que o usuário clique e navegue para dentro do serviço. Isso aumenta a chance de o usuário seguir um caminho errado sem perceber e sem ter como voltar de forma guiada.

---

### Visibilidade e Reconhecimento

O designer deve tornar visíveis as possibilidades de execução e avaliação disponíveis ao usuário. Antes de executar uma ação, o usuário precisa saber o que é possível realizar e como as ações devem ser feitas, sem ser obrigado a memorizar etapas [1].

**Violação identificada no site da Educação DF:**
A página da Carta de Serviços não deixa claro para o usuário quais serviços estão disponíveis de forma digital e quais exigem atendimento presencial. As dez categorias são apresentadas apenas como links textuais simples, sem ícones, descrições ou qualquer indicador visual que comunique o tipo de serviço ou canal de atendimento disponível. O usuário é obrigado a clicar em cada item para descobrir o que existe dentro de cada categoria.

---

### Encontrabilidade

A encontrabilidade diz respeito à facilidade de localizar informações dentro do site, tanto por usuários que já o conhecem quanto por aqueles que chegam de fora. Esse princípio transforma a interação com a plataforma em uma experiência rápida e eficaz.

**Violação identificada no site da Educação DF:**
A funcionalidade de remanejamento escolar não possui uma entrada direta e destacada na página da Carta de Serviços. O usuário precisa saber previamente que o remanejamento está categorizado dentro de "Matrícula" ou "Vida escolar" para encontrá-lo — uma associação que não é óbvia. Não há mecanismo de busca contextual dentro da Carta de Serviços, nem tags ou palavras-chave que ajudem o usuário a localizar o serviço desejado sem precisar explorar todas as categorias.

---

### Correspondência com as Expectativas dos Usuários

Devem-se explorar os mapeamentos naturais entre as tarefas e os controles utilizados para manipulá-las no sistema, de forma que o comportamento do site corresponda ao que o usuário naturalmente espera ao acessá-lo [1].

**Violação identificada no site da Educação DF:**
O item "Serviços" no menu principal leva a uma página intermediária que contém apenas o subitem "Carta de Serviços", o que frustra a expectativa do usuário de encontrar diretamente os serviços disponíveis ao clicar nesse menu. A presença de um nível de navegação extra sem conteúdo adicional relevante contraria o comportamento esperado em sites governamentais, onde "Serviços" normalmente aponta diretamente para uma lista de serviços disponíveis.

---

### Antecipação das Necessidades do Usuário

As aplicações devem tentar prever o que o usuário quer e precisa, em vez de esperar que ele busque informações ou invoque ferramentas por conta própria. O designer deve fornecer todas as informações e recursos necessários para cada passo do processo [1].

**Violação identificada no site da Educação DF:**
A página da Carta de Serviços não exibe proativamente informações sobre prazos vigentes, como o calendário de remanejamento escolar ou períodos de matrícula em aberto. Um usuário que acessa o site fora do período de remanejamento não recebe qualquer aviso sobre quando o próximo período se inicia, sendo obrigado a navegar por outras seções do site para encontrar essa informação por conta própria.

---

### Equilíbrio entre Controle e Liberdade do Usuário

Ao oferecer ao usuário a sensação de controle sobre o sistema, ele aprende mais rapidamente e desenvolve confiança na plataforma. Sem limitações adequadas, o usuário pode se sentir perdido diante de muitos estímulos [1].

**Violação identificada no site da Educação DF:**
O menu de navegação principal apresenta mais de 40 itens e subitens distribuídos em múltiplos níveis, sobrecarregando o usuário com opções em excesso sem qualquer mecanismo de filtragem ou personalização por perfil (cidadão, servidor, estudante, responsável). Essa ausência de segmentação por tipo de usuário retira o controle do cidadão comum, que se vê obrigado a navegar por conteúdo institucional e administrativo que não é relevante para sua necessidade imediata.

---

## Conclusão

É essencial que um bom projeto de sistema tenha princípios bem organizados e orientados ao bem-estar de seus usuários. A análise do site da Secretaria de Estado de Educação do Distrito Federal revelou violações recorrentes, especialmente nos princípios de simplicidade, encontrabilidade, eficiência do usuário e antecipação das necessidades. As violações identificadas serão utilizadas como base para as propostas de redesign da funcionalidade analisada.

## Referências Bibliográficas

> <a id="REF1">1.</a> BARBOSA, S. D. J.; SILVA, B. S. da; SILVEIRA, M. S.; GASPARINI, I.; DARIN, T.; BARBOSA, G. D. J. (2021). *Interação Humano-Computador e Experiência do Usuário*. Autopublicação. ISBN: 978-65-00-19677-1.

## Histórico de versão

| Versão | Data       | Descrição                              | Autor(es)                                    | Revisor(es) |
| ------ | ---------- | -------------------------------------- | -------------------------------------------- | ----------- |
| `1.0`  | 10/05/2026 | Criação do documento                   | [Ígor Veras](https://github.com/igorvdaniel) |             |