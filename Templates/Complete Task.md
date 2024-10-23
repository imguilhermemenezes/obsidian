<%*
// Caminho do arquivo Kanban
const kanbanFile = app.vault.getAbstractFileByPath('Agenda.md');

// Obter o título da daily note (data da nota)
const title = tp.date.now('YYYY-MM-DD');

// Ler o conteúdo atual do arquivo Kanban
const content = await app.vault.read(kanbanFile);

// Marcar o cartão correspondente como completado
const updatedContent = content.replace(`- [ ] ${title}`, `- [x] ${title}`);
await app.vault.modify(kanbanFile, updatedContent);
%>
