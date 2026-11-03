# DB Recovery Lab

Documentação técnica e laboratório didáctico em português sobre diagnóstico, recuperação e validação de MySQL/MariaDB no Windows, com foco no XAMPP.

## GitHub Pages

O repositório publica a partir da branch `main` e da pasta `/(root)`. URL previsto: https://egaslemos-gif.github.io/db-recovery-lab/

## Conteúdo didáctico

- Segurança, backups e fundamentos MySQL/MariaDB/XAMPP.
- Diagnóstico, logs, conflitos de portas, mecanismos Aria e InnoDB.
- Procedimentos de backup, restauro, validação e prevenção.
- Recovery Wizard para triagem orientada por sintomas.
- Terminal Simulator fictício, sem acesso à shell, rede ou sistema de ficheiros.
- Recovery Case Studies e análise de incidentes.
- DB Recovery Challenges e Knowledge Assessment com feedback automático.
- Learning Progress local no navegador.
- Instructor Mode com notas e gabarito.

## Estrutura técnica

- `index.html`: carregador estático que reconstrói a página integral.
- `payload/part-01.txt` a `payload/part-09.txt`: fragmentos Base64 do HTML comprimido em gzip.
- `references/official-sources.md`: documentação oficial de referência.

Não requer backend, Node.js, instalação de dependências ou processo de build. A página completa é descomprimida no navegador via `DecompressionStream`.

## Segurança

Faça uma cópia integral da pasta de dados antes de qualquer intervenção. Não execute `aria_chk` com MariaDB em funcionamento. `innodb_force_recovery` é um mecanismo de emergência para extracção de dados, não uma ferramenta de reparação. Adapte os procedimentos à versão instalada.

O Terminal Simulator é exclusivamente didáctico. O progresso guardado em `localStorage` é local ao navegador e não identifica nem sincroniza estudantes.
