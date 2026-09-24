# Portfólio de Sérgio Guthyerres

Página estática, sem framework e sem build. Um arquivo `index.html` com CSS e JS embutidos.

## Publicar no GitHub Pages (grátis, ~5 minutos)

1. **Crie um repositório chamado exatamente `SergioGuthyerres.github.io`**. O nome precisa ser igual ao seu usuário, com `.github.io` no fim. É isso que faz o GitHub servir na raiz do domínio.

2. **Suba os arquivos:**
   ```bash
   git init
   git add .
   git commit -m "portfolio: versão inicial"
   git branch -M main
   git remote add origin https://github.com/SergioGuthyerres/SergioGuthyerres.github.io.git
   git push -u origin main
   ```

3. **Ative o Pages:** no repositório, *Settings → Pages → Source → Deploy from a branch → main / (root)*.

4. Aguarde de 1 a 2 minutos. O site fica em **https://sergioguthyerres.github.io**

A partir daí, todo `git push` republica.

## Antes de divulgar

- [ ] **Confira o PDF do currículo na raiz.** O botão "Currículo (PDF)" do topo aponta para `CurriculoSergioGuthyerresPT.pdf`. Se você renomear o arquivo, ajuste o link no `index.html`.
- [ ] **Confira os links dos projetos.** Todos abrem em aba nova.
- [ ] **Teste no celular.** A página é responsiva, mas veja com seus olhos.
- [ ] **Passe a URL no [Post Inspector do LinkedIn](https://www.linkedin.com/post-inspector/).** O `github.io` não tem o problema de TLS do `workers.dev`, então aqui o preview deve funcionar, e aí você finalmente consegue um link nos Destaques.

## Manutenção

O conteúdo está em HTML puro e legível. Para adicionar um projeto, copie um bloco `<article class="card">` e troque o texto. Os selos de status são as classes:

| Classe | Rótulo sugerido |
|---|---|
| `b-live` | Em produção |
| `b-wip` | Em desenvolvimento |
| `b-done` | Concluído |
| `b-mute` | Em pausa / privado |

O tema claro/escuro segue a preferência do sistema e pode ser alternado pelo botão da barra superior; a escolha fica salva no navegador.

## Quando você tiver um domínio próprio

1. Crie um arquivo `CNAME` na raiz com o domínio dentro (só o domínio, uma linha).
2. Aponte o DNS para o GitHub Pages.
3. Troque `sergioguthyerres.github.io` pelo domínio novo nas meta tags `og:url` e `og:image` do `index.html`.

Nada mais muda.
