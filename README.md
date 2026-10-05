# Corretor de Simulados — Escola Estadual João Paulo II

Versão 2 — correção por câmera/OMR para os cartões atuais de 30 e 35 questões.

## Principais recursos
- Leitura por câmera ou foto dos cartões de resposta.
- Reconhecimento das marcações A, B, C e D.
- Identificação de branco e sinalização de marcação ambígua.
- Leitura baseada nos 4 marcadores pretos presentes na área de respostas.
- Compatível com o layout atual de 30 questões e com o layout de 35 questões.
- Correção dos 5 simulados cadastrados.
- Cadastro individual e importação de alunos por CSV/XLSX.
- Gabaritos manuais ou por CSV.
- Correção em sequência: salvar e passar ao próximo aluno sem fechar a câmera.
- Evita duplicar a correção do mesmo aluno no mesmo simulado: uma nova leitura atualiza a anterior.
- Resultados por aluno, turma, simulado e disciplina.
- Análise questão a questão.
- Backup/restauração em JSON.
- Exportação de resultados em CSV.
- Impressão de relatório.
- PWA instalável em celular.

## Uso no computador
1. Extraia o ZIP.
2. Execute `start-server.bat`.
3. Abra o endereço indicado pelo servidor.
4. Cadastre os alunos e os gabaritos.
5. Entre em **Corrigir cartões**.
6. Escolha o simulado, turma e aluno.
7. Abra a câmera e enquadre **somente um cartão**, mantendo os quatro quadrados pretos visíveis.
8. Capture e revise as questões amarelas, se houver.
9. Salve ou use **Salvar e próximo aluno**.

## Uso no celular
Publique a pasta em um servidor HTTPS, por exemplo GitHub Pages. O navegador precisa de HTTPS para liberar a câmera. Depois, abra o site no celular e permita o acesso à câmera. O aplicativo pode ser instalado na tela inicial como PWA.

## Importante sobre a leitura
O leitor não utiliza OCR do nome escrito à mão. Nos cartões atuais, o aluno é selecionado no aplicativo. A leitura das alternativas usa os marcadores pretos para calcular a posição das bolhas. Se uma marcação for duvidosa, ela é enviada para revisão manual em vez de ser automaticamente considerada como resposta.

## QR Code
Os QR Codes dos 5 simulados ficam em `assets/qrs/`. O formato usado é `JPII|SIMULADO|1` até `JPII|SIMULADO|5`.
