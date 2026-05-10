# Guia de Estilo - Matrículas DF

> Documento de diretrizes de design para o sistema de matrículas da Secretaria de Educação do Distrito Federal - IHC/UnB 2026

---

## Introdução

Este guia de estilo estabelece as diretrizes visuais e de interação para o redesign do sistema de matrículas online da Secretaria de Estado de Educação do
Distrito Federal (SEEDF). O sistema tem como função principal permitir que responsáveis legais realizem a matrícula e rematrícula de estudantes da rede pública de ensino do DF. 

#### Organização e conteúdo do guia de estilo

A organização do guia de estilo seguirá a proposta de Marcus e Mayhew, conforme referenciado em Barbosa:

1. Introdução
2. Resultados de análise 
3. Elementos de interface
4. Elementos de interação
5. Elementos de ação
6. Vocabulário e padrões

#### Público-alvo do guia de estilo

Este guia foi elaborado pelos estudantes da disciplina de Interação Humano-Computador da Universidade de Brasília para orientar decisões de design e
desenvolvimento do sistema de matrículas do DF. Pode ser utilizado por qualquer equipe envolvida com o produto.

#### Como utilizar o guia

Este guia deve ser utilizado como referência para tomar decisões de design durante todo o ciclo de vida do projeto, incluindo prototipação, produção e
manutenção.

#### Como manter o guia

A equipe deve atualizar o guia sempre que novas decisões forem tomadas ou quando houver mudanças que contrariem o que foi previamente descrito.

---

## 2. Resultados de análise 

#### Descrição o ambiente de trabalho do usuário

O sistema de matrículas do DF é primariamente acessado via computadores (desktops e notebooks) em lan houses, escolas e residências. Dispositivos móveis
representam uma parcela crescente dos acessos, especialmente por responsáveis que utilizam smartphones Android de entrada.

**Dispositivos mais utilizados:**

- Desktop / Notebook
- Smartphone Android (acesso secundário, em crescimento)
- Tablet (uso esporádico)

**Contexto de uso:**

- Conexões instáveis (3G/4G em zonas periféricas)
- Picos de acesso nos períodos de matrícula (janeiro e julho) 
- Mútiplos perfis de usuário com diferentes níveis de letramento digital

---

## 3. ELementos de interface

#### Paleta de cores

| Nome | Hex | Uso |
| ---|---|---|
| Azul Governo (primária) | `#1351B4` | Botões principais, links, ações primárias |
| Azul Hover | `#155BCB` | Estado hover de botões primpários |
| Azul Escuro (secundária) | `#071D41` | Cabeçalhos, rodapé, destaques |
| Verde Sucesso | `#1668821` | Confirmações, matrículas concluídas |
| Vermelho Erro | `#DC3545` | Erros, campos obrigatórios não preenchidos |
| Cinza Fundo | `#F8F8F8` | Fundo das páginas internas | 
| Branco | `#FFFFFF` | Fundo de cards e formulários |

> A paleta segue o padrão de Design System Gov.br, garantindo consistência com demais serviços digitais do governo federal.


#### Tipografia

| Uso | Fonte | Tamanho | Peso |
|---|---|---|---|
| Fonte principal | Rawline (Gov.br) / Raleway | — | — |
| Título H1 | Rawline | 32px | 500 |
| Título H2 | Rawline | 24px | 500 |
| Título H3 | Rawline | 20px | 500 |
| Corpo de texto | Rawline | 16px | 400 |
| Rótulo de formulário | Rawline | 14px | 400 |
| Texto auxiliar | Rawline | 12px | 400 |

---

## 4. ELementos de interação

##### Estilos de interação

Os usuários interagem com o sistema para: buscar escola por localização, preencher dados do estudante, anexar documentos, acompanhar o status da
matrícula e receber confirmação. Todas as interações se dão por botões, formulários e mensagens de feedback.

##### Seleção de um estilo

O sistema deve adotar uma interface limpa e orientada a tarefas, com foco no fluxo de matrículas. Informações secundárias devem ser separadas da área
funcional principal, evitando poluição visual.

##### Fluxo principal (wizard)

1. Login / identificação do responsável 
2. Dados do responsável legal
3. Dados do estudante
4. Escolha de escola e turno
5. Envio de documentos
6. Revisão e confirmação
7. Emissão do comprovante

##### Aceleradores / Teclas de atalho

O sistema atual não possui teclas de atalho. Recomenda-se implementar: `Tab` para navegação entre campos, `Enter` para confirmar e `Esc` para fechar modais.

---

## 5. Elementos de ação

##### Preenchimento de campos

Os formulários exigem inserção manual de dados. Todos os campos devem apresentar:

- Rótulo visível acima do campo
- Placeholder com exemplo de preenchimento (ex.: `000.000.000.00` para CPF)
- Mensagem de erro clara e próxima ao campo com falha
- Indicação visual de campo obrigatório (asterisco `*`)

##### Seleção

- **Etapa de ensino:** Educação Infantil, Ensino Fundamental, Ensino Médio
- **Turno:** Matutino, Verspertino, Noturno, Integral
- **Região Administrativa:** lista completa das RAs do DF
- **Escola de preferência:** Filtrada por RA e etapa

##### Ativação

Hierarquia de botões:

- **Primário** (`#1351B4`): ação principal da tela (ex.: "Confirmar matrícula","Avançar")
- **Secundário** (borda + texto azul): ação alternativa (ex.: "Voltar", "Salvar rascunho")
- **Destruitivo** (`#DC3545`): ação irrerversível (ex.: "Cancelar solicitação")

---

## 6. Vocabulário e padrões

##### Terminologia

| Usar | Evitar |
|---|---|
| Responsável legal | Tutor, guardião |
| Estudante | Aluno, menor |
| Etapa de esnino | Nível, série |
| Solicitação de matrícula | Request, pedido |
| Comprovante | Voucher, recibo |
| Região Administrativa (RA) | Bairro, cidade-satélite |

##### Tipos de tela

- **Telas de fluxo:** cabeçalho com indicador de progresso, área de formulário centralizada, rodapé com botões de navegação
- **Telas de suporte:** cabeçalho institucional, área de conteúdo informativo, links para FAQ e atendimento

##### Sequências de diálogos

Mensagens de feedback seguem o padrão:


- **Sucesso:** fundo verde `#168821`, ícone de check, texto positivo
- **Atenção:** fundo amarelo `#FFCD07`, ícone de alerta, orientação clara
- **Erro:** fundo vermelho `#DC3445`, ícone de erro, instrução de correção

##### Acessibilidade

Seguindo WCAG 2.1 nível AA:

- Constraste mínimo de 4,5:1 entre texto e fundo
- Compatibilidade com leitores de tela (`aria-label`, `role`, `alt`) 
- Navegação completa por teclado
- Textos alternativos em todas as imagens e ícones funcinais

---

## Referências Bibliográficas

> 1. MARCUS, A. *Graphic design for electronic documents and user interfaces.* ACM, New York, 1991.
>
> 2. MAYHEW, D. J. *The Usability Engineering Lifecycle.* Morgan Kaufmann, 1999.
>
> 3. BARBOSA, S. D. J.; SILVA, B. S. *Interação Humano-Computador.* Rio de Janeiro: Elsevier, 2011.
>
> 4. BRASIL. *Padrão Digital de Governo — Design System Gov.br.* Disponível em: https://www.gov.br/ds

---


 Versão | Data | Descrição | Autor(es) | Revisor(es) |
|---|---|---|---|---|
| `1.0` | 10/05/2026 | Criação da página Guia de Estilo Inicial | [Joao Guilherme](https://github.com/JoaoGSantana10) | |