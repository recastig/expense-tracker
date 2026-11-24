# Despesas — Controle de orçamento pessoal

Aplicação web de controle de despesas desenvolvida com **HTML, CSS e JavaScript puro (Vanilla JS)**. Permite definir um orçamento, adicionar e remover gastos e acompanhar estatísticas atualizadas na própria interface.

## Funcionalidades

- Definição do valor do orçamento.
- Cadastro de despesas por categoria e valor, por meio de um formulário modal.
- Exclusão individual de despesas e opção de redefinir os dados para os valores de exemplo.
- Cálculo de despesas totais, média por lançamento, saldo disponível, categoria com maior gasto e totais por categoria.
- Indicador visual do saldo, com mudança de cor conforme a relação entre saldo e orçamento.
- Persistência do orçamento e dos lançamentos no `localStorage` do navegador.

As categorias disponíveis são **Mercado, Comer fora, Transporte, Casa e Assinaturas**. Na primeira execução, a aplicação inicia com lançamentos de exemplo; a opção **Limpar tudo** restaura esses lançamentos iniciais em vez de manter a lista permanentemente vazia.

## Tecnologias

| Tecnologia | Uso |
| --- | --- |
| HTML5 | Estrutura da página e formulários |
| CSS3 | Layout e estilos organizados em blocos |
| JavaScript | Manipulação do DOM, eventos, cálculos e atualização da interface |
| Web Storage API | Armazenamento local do orçamento e das despesas |

Não utiliza frameworks, backend ou banco de dados externo.

## Como executar

1. Baixe ou clone o repositório.
2. Abra o arquivo `index.html` no navegador.
3. Defina um orçamento e utilize **Nova Despesa** para registrar os lançamentos.

Não é necessário instalar dependências ou executar um servidor de desenvolvimento.

## Organização do projeto

```text
expense-tracker/
├── blocks/                # Estilos por componente/bloco
├── images/                # Ícones
├── pages/index.css        # Entrada dos estilos
├── scripts/
│   ├── calculations.js    # Cálculos e dados das despesas
│   ├── handle-html.js     # Renderização e eventos do DOM
│   └── index.js           # Inicialização e localStorage
├── vendor/                # Fontes e normalização de estilos
├── index.html
└── README.md
```

## Aprendizados técnicos

O projeto exercita a separação entre **lógica de cálculo**, **manipulação da interface** e **inicialização**, além do uso de eventos, arrays, formulários e persistência de dados no navegador.

## Limitações e possíveis melhorias

- Os dados ficam no navegador utilizado; não há sincronização entre dispositivos nem contas de usuário.
- O cadastro de despesas poderia ter validação mais rigorosa de valores antes de aceitá-los.
- A redefinição atualmente restaura os lançamentos de exemplo; uma evolução seria permitir limpar a lista completamente.
- Uma próxima versão poderia disponibilizar exportação dos lançamentos e gráficos de evolução.

## Autoria

Projeto educacional desenvolvido por **Renan Castiglioni** durante estudos de desenvolvimento web.
