# Controle de Ponto (Vite + React + Tailwind)

## Rodar local
1. Baixe o zip e extraia.
2. No terminal, dentro da pasta:
   ```bash
   npm install
   npm run dev
   ```
3. Abra o endereço indicado (geralmente http://localhost:5173).

## Gerar build de produção
```bash
npm run build
npm run preview
```
Os arquivos finais ficam em `dist/`.

## Publicar (3 opções fáceis)
**Vercel**
- Crie uma conta em vercel.com
- `vercel` (CLI) ou conecte seu GitHub e faça o import do repositório com este projeto.
- Framework: Vite; Build: `npm run build`; Output: `dist`.

**Netlify**
- netlify.com → New site from Git → selecione seu repo.
- Build command: `npm run build`; Publish directory: `dist`.

**GitHub Pages (estático)**
- Rode `npm run build`.
- Suba o conteúdo de `dist/` para a branch `gh-pages` e habilite Pages.
- OU use a action oficial de Pages para projetos Vite.

## Observações
- Dados ficam no `localStorage` do navegador (LS_KEY: `controle-ponto-v3`). Não há backend.
- Exporta CSV, XLSX e PDF.
- Calendário começa no domingo. Finais de semana e feriados **não** contam nos totais; **ponto facultativo** (★) NÃO exclui horas.
- Assinatura do Gestor bloqueia edição do mês; Colaborador ainda pode assinar.
