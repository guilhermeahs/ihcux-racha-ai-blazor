# ihcux-racha-ai-blazor

Projeto em Blazor para representar o dashboard principal do aplicativo RachaAí.

## Implementação Blazor

A tela foi organizada com uma hierarquia visual simples: os cards de resumo aparecem no topo para mostrar rapidamente o saldo geral, o total a receber e o total a pagar. A lista de grupos fica logo abaixo, usando cards individuais para facilitar a leitura das pendências.

O componente `GrupoCard.razor` recebe um objeto `Grupo` e exibe o nome, a categoria e o valor pendente. As cores verde e vermelha ajudam o usuário a identificar se ele tem crédito ou dívida em cada grupo.

## Dificuldade Técnica

A maior dificuldade foi separar a responsabilidade da página e do componente. A página `Dashboard.razor` controla a lista, a busca e os totais, enquanto o `GrupoCard.razor` fica responsável apenas pela exibição de cada grupo.

## Funcionalidades

- Cards de resumo financeiro
- Lista de grupos ativos
- Componente reutilizável para os grupos
- Botão de novo gasto
- Busca por nome ou categoria
- Mensagem para lista vazia
