# Da Ficha à Planilha

Sequência didática interativa de letramento em dados para estudantes do 6º ao 8º ano do Ensino Fundamental. A atividade parte de fichas de personagens fictícios e chega a uma tabela que a turma pode organizar, validar e analisar.

| Aula | Atividade |
| --- | --- |
| 1. Organização tabular | Transformar fichas em registros e distinguir linhas de colunas. |
| 2. Tipos e validação | Classificar campos e testar quais valores podem ser cadastrados. |
| 3. Coleta e análise | Cadastrar personagens, ordenar por idade ou altura, filtrar pela posse de pet e exportar os registros em CSV. |

## Como usar

- Abra a [atividade publicada no Google Apps Script](https://script.google.com/a/macros/escola.pr.gov.br/s/AKfycbzEWeEpENrUWlYdjp7LmgCYybjsmtA1HJyTjlt7kbbpYMgCHrZtKq35U-ASXGmtHyuUwQ/exec).
- Para usar uma cópia local, baixe [index.html](index.html) e abra o arquivo no navegador. As atividades funcionam sem instalação. O [vídeo introdutório](https://www.youtube.com/watch?v=1TLM2g5_114) requer internet.
- Os cadastros ficam em memória durante a sessão. Exporte o CSV antes de fechar ou recarregar a página. A exportação inclui todos os registros da sessão, inclusive os que o filtro ocultou.

## Como adaptar

O arquivo `index.html` reúne HTML, CSS e JavaScript. Você pode editar as fichas, os campos e as regras de validação e abrir sua cópia no navegador para testar as três etapas. Use dados fictícios nos exemplos de cadastro.

Para publicar sua cópia no Google Apps Script, crie um arquivo HTML chamado `Index` e cole o conteúdo de `index.html`. No arquivo `Code.gs`, adicione:

```javascript
function doGet() {
  return HtmlService.createHtmlOutputFromFile('Index');
}
```

Implante o projeto como aplicativo da Web e escolha o acesso conforme as permissões da sua conta.

## Créditos e licença

Proposta didática de André José de Souza, Joice Maiara de Souza Bernardo e Regiane Pascoal Martire Ferreira. Código desenvolvido por André José de Souza e distribuído sob a [licença MIT](LICENSE). A licença deste repositório se aplica ao código da aplicação.
