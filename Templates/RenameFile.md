<%*
const version = "v001-001";
const now = tp.date.now("YYYYMMDD_HHmmss", 0);
const fileName = `character_lorebook_${version}_${now}`;
await tp.file.rename(fileName);
%>