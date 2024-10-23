### Manhã

- [ ] 06:00 Acordar e Tomar Banho
- [ ] 06:40 Levar meu irmão para a escola
- [ ] 07:20 Tomar banho
- [ ] 07:30 Ir para a academia
- [ ] 09:00 Tomar café
- [ ] 09:30 Estudar __inglês
- [ ] 10:00 Procrastinar | Estudar __Música
- [ ] 10:50 Buscar meu irmão da escola
- [ ] 11:30 Afazer em casa
- [ ] 12:00 Almoçar
### Tarde

- [ ] 12:30 Estudar __desenho | educação financeira
- [ ] 14:00 Estudar __Programação
- [ ] 16:00 Me arrumar para a faculdade
- [ ] 16:50 Sair para a faculdade
### Noite

- [ ] 22:00 Chegar em casa, tomar banho e Jantar
- [ ] 22:30 Estudar __coreano
- [ ] 23:00 Procrastinar
- [ ] 00:00 Dormir

<%*
// Caminho do arquivo Kanban (ajuste o nome conforme necessário)
const kanbanFile = app.vault.getAbstractFileByPath('Agenda.md');

// Formatar a data da nota diária
const today = tp.date.now('yyyy/MM/dd');

// Tarefas padrão que deseja adicionar
const tasks = `- [ ] Tarefa 1\n- [ ] Tarefa 2`;

// Formato para a seção do Kanban
const dailySection = `## ${today}\n${tasks}\n`;

// Ler o conteúdo atual do arquivo Kanban
const content = await app.vault.read(kanbanFile);

// Adiciona as tarefas no arquivo Kanban
if (content.includes("## Daily")) {
    const updatedContent = content.replace("## Daily", `## Daily\n${dailySection}`);
    await app.vault.modify(kanbanFile, updatedContent);
} else {
    await app.vault.modify(kanbanFile, content + `\n## Daily\n${dailySection}`);
}
%>

