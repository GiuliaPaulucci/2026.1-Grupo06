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

Este guia foi elaborado pelos estudantes da disciplina de Interação Humano-Computador da Universidade de Brasília para orientar decisões de design e desenvolvimento do sistema de matrículas do DF. Pode ser utilizado por qualquer equipe envolvida com o produto.

#### Como utilizar o guia

Este guia deve ser utilizado como referência para tomar decisões de design durante todo o ciclo de vida do projeto, incluindo prototipação, produção e manutenção.

#### Como manter o guia

A equipe deve atualizar o guia sempre que novas decisões forem tomadas ou quando houver mudanças que contrariem o que foi previamente descrito.

---

## 2. Resultados de análise 

#### Descrição o ambiente de trabalho do usuário

O sistema de matrículas do DF é primariamente acessado via computadores (desktops e notebooks) em lan houses, escolas e residências. Dispositivos móveis representam uma parcela crescente dos acessos, especialmente por responsáveis que utilizam smartphones Android de entrada.

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

Os usuários interagem com o sistema para: buscar escola por localização, preencher dados do estudante, anexar documentos, acompanhar o status da matrícula e receber confirmação. Todas as interações se dão por botões, formulários e mensagens de feedback.

##### Seleção de um estilo