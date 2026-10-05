# Corretor de Simulados — Escola Estadual João Paulo II

Sistema web/PWA para cadastro de alunos, configuração de simulados, gabaritos por série, geração de cartões-resposta, leitura de QR Code e correção por câmera com reconhecimento OMR.

## Funcionalidades

- 5 modelos de simulado pré-configurados.
- Gabarito separado para 6º, 7º, 8º e 9º ano.
- Cartão-resposta de 30 ou 35 questões.
- QR Code identificando o simulado e a série.
- Impressão do cartão-resposta e do QR Code.
- Correção por câmera usando leitura OMR.
- Identificação de respostas em branco, duplas/ambíguas e marcações válidas.
- Resultado com acertos, erros, brancos e percentual.
- Cadastro individual e importação de alunos por CSV/XLSX.
- Histórico e relatórios.
- Interface adaptada para computador e celular.
- PWA instalável.
- Integração opcional com Supabase para sincronização.

## Publicação no GitHub Pages

1. Crie um repositório no GitHub.
2. Envie todo o conteúdo desta pasta para a branch `main`.
3. No GitHub, abra **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/ (root)`.
6. Salve e aguarde a publicação.

O arquivo `index.html` está na raiz do projeto para que o GitHub Pages consiga servir o sistema diretamente.

## Importante sobre dados e Supabase

Não coloque senhas, service keys ou outras credenciais privadas no repositório. O GitHub recomenda não enviar informações sensíveis para o repositório. citeturn0search9

A configuração do Supabase é feita dentro do próprio sistema. O arquivo `supabase-schema.sql` contém o esquema de banco preparado para a sincronização.

## Estrutura

- `index.html` — aplicação principal.
- `assets/logo-escola.png` — logomarca da escola.
- `manifest.webmanifest` — configuração PWA.
- `sw.js` — service worker/offline cache.
- `supabase-schema.sql` — estrutura do banco Supabase.
- `start-server.bat` — servidor local para testes no Windows.
- `start-server.ps1` — servidor local PowerShell.

## Escola

**Escola Estadual João Paulo II**  
**DRE Maracanã**
