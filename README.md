# DB Recovery Lab

Portal técnico e laboratório didáctico em português sobre diagnóstico, recuperação e validação de MySQL/MariaDB em Windows, com foco no XAMPP.

## Publicação

O GitHub Pages está configurado para publicar a branch `main` a partir da raiz `/(root)`.

URL do projecto: https://egaslemos-gif.github.io/db-recovery-lab/

## Conteúdo

- Documentação técnica: segurança, backups, fundamentos de MySQL/MariaDB/XAMPP, diagnóstico, leitura de logs, portas, Aria, InnoDB, backup/restauro, tabelas de sistema, validação e prevenção.
- Recovery Wizard: triagem por sintomas.
- Terminal Simulator: terminal didáctico simulado, sem execução de comandos reais.
- Recovery Case Studies: estudos de caso e decisões de recuperação.
- DB Recovery Challenges: exercícios com feedback.
- Knowledge Assessment: avaliação de conhecimentos.
- Learning Progress: progresso local no navegador.
- Instructor Mode: notas para o docente e respostas.

## Estrutura

- `index.html`: carregador estático do laboratório.
- `payload/part-01.txt` a `payload/part-12.txt`: fragmentos Base64 do HTML original, codificado em UTF-8.
- `references/official-sources.md`: referências oficiais.

O carregador reúne os fragmentos e apresenta a página integral no navegador. Não requer backend, Node.js ou processo de build.

## Segurança

Faça uma cópia integral da pasta de dados antes de qualquer intervenção. Não execute `aria_chk` com o MariaDB em funcionamento. `innodb_force_recovery` é um mecanismo de emergência para extracção de dados, não uma ferramenta de reparação. Adapte os procedimentos à versão instalada.

O Terminal Simulator é exclusivamente didáctico e não tem acesso à shell, rede ou sistema de ficheiros. O progresso guardado em `localStorage` é local ao navegador.
