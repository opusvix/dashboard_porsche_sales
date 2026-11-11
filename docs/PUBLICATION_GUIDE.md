# Guia completo de publicação

Este guia cobre três entregas:

1. criação do repositório `dashboard_porsche_sales` no GitHub;
2. inclusão do projeto em `https://opusvix.github.io`;
3. publicação e destaque do post no LinkedIn.

---

## 1. Publicar o projeto no GitHub

### 1.1 Preparar os arquivos

1. Baixe e extraia o pacote recebido.
2. Abra a pasta `dashboard_porsche_sales`.
3. Confirme que ela contém:
   - `README.md`;
   - pasta `assets` com a capa;
   - pasta `docs` com os textos do portfólio, LinkedIn e este guia.
4. Não altere os nomes dos arquivos antes do primeiro envio. Os caminhos utilizados no README dependem dessa estrutura.

### 1.2 Criar o repositório

1. Acesse `https://github.com/new` conectado à conta `opusvix`.
2. Em **Repository name**, informe exatamente:

   ```text
   dashboard_porsche_sales
   ```

3. Em **Description**, use:

   ```text
   Dashboard executivo de vendas Porsche com KPIs, comparação temporal, drill-through, insights e detalhamento transacional.
   ```

4. Marque o repositório como **Public**.
5. Como os arquivos já estão prontos, deixe desmarcadas as opções:
   - Add a README file;
   - Add .gitignore;
   - Choose a license.
6. Clique em **Create repository**.

### 1.3 Método recomendado: publicar com Git

No Windows, abra o PowerShell dentro da pasta extraída. Uma forma simples é abrir a pasta no Explorador de Arquivos, clicar na barra de endereço, digitar `powershell` e pressionar Enter.

Execute cada comando separadamente:

```powershell
git init
git add .
git commit -m "docs: publica projeto Porsche Sales Intelligence"
git branch -M main
git remote add origin https://github.com/opusvix/dashboard_porsche_sales.git
git push -u origin main
```

Se o Git solicitar autenticação, conclua o login pelo navegador ou pelo Git Credential Manager. Não informe senha ou token dentro dos arquivos do projeto.

### 1.4 Método alternativo: upload pelo navegador

Se preferir não utilizar Git:

1. Abra o repositório recém-criado.
2. Clique em **uploading an existing file** ou em **Add file → Upload files**.
3. Arraste o conteúdo da pasta `dashboard_porsche_sales` para a área de upload.
4. Confirme que `README.md`, `assets` e `docs` aparecem na lista.
5. Em **Commit changes**, informe:

   ```text
   docs: publica projeto Porsche Sales Intelligence
   ```

6. Clique em **Commit changes**.

### 1.5 Configurar a apresentação do repositório

Na página principal do repositório:

1. Localize a seção **About**.
2. Clique no ícone de edição.
3. Use a descrição:

   ```text
   Dashboard executivo de vendas Porsche com KPIs, comparação temporal, drill-through, insights e exportação CSV.
   ```

4. Em **Website**, informe:

   ```text
   https://opusvix.github.io/dashboard_porsche_sales/
   ```

5. Em **Topics**, adicione:

   ```text
   data-analytics
   business-intelligence
   dashboard
   react
   typescript
   data-visualization
   portfolio-project
   ai-assisted-development
   ```

6. Salve as alterações.

### 1.6 Validar o repositório

Abra:

```text
https://github.com/opusvix/dashboard_porsche_sales
```

Verifique:

- a capa é exibida no topo do README;
- o link **Acesse o dashboard** abre a aplicação;
- os arquivos da pasta `docs` podem ser abertos;
- a seção About mostra o link do dashboard;
- a declaração de desenvolvimento assistido por IA está visível;
- não existem dados pessoais, credenciais ou arquivos temporários.

---

## 2. Adicionar o projeto ao portfólio

O portfólio atual apresenta os projetos com imagem, título, descrição, tecnologias e links para GitHub e dashboard. O novo item foi preparado no mesmo formato.

### 2.1 Localizar a origem publicada pelo GitHub Pages

1. Acesse o repositório responsável por `https://opusvix.github.io`.
2. Abra **Settings → Pages**.
3. Em **Build and deployment**, verifique:
   - a branch utilizada, normalmente `main`;
   - a pasta de publicação, normalmente `/(root)` ou `/docs`.
4. Retorne à aba **Code** e abra essa branch e pasta.

### 2.2 Encontrar o arquivo da página inicial

Procure nesta ordem:

1. `index.md`;
2. `README.md`;
3. `index.html`.

Abra o arquivo e pesquise pelo texto:

```text
Projetos em Destaque
```

O arquivo que contém esse título é o local onde o novo projeto deve ser inserido.

### 2.3 Enviar a imagem

1. Abra a pasta `assets` do repositório do portfólio.
2. Clique em **Add file → Upload files**.
3. Envie:

   ```text
   dashboard-porsche-sales-cover.png
   ```

4. Use a mensagem de commit:

   ```text
   feat: adiciona capa do dashboard Porsche Sales
   ```

5. Confirme o commit na branch de publicação.

### 2.4 Inserir o projeto

1. Abra o arquivo identificado na etapa 2.2.
2. Clique no ícone de edição.
3. Localize a seção **Projetos em Destaque**.
4. Para dar maior visibilidade ao projeto, insira-o como o primeiro item da seção.
5. Abra `docs/PORTFOLIO_ENTRY.md` deste pacote.
6. Copie o bloco **Versão recomendada — Markdown/Jekyll**.
7. Cole no arquivo do portfólio.
8. Garanta que exista uma linha em branco antes e depois do bloco.
9. Faça o commit com a mensagem:

   ```text
   feat: destaca dashboard Porsche Sales Intelligence
   ```

Se o arquivo inicial estiver em HTML, utilize a seção **Versão alternativa — HTML** do mesmo documento.

### 2.5 Acompanhar a publicação

1. Abra a aba **Actions** do repositório do portfólio.
2. Aguarde o workflow de GitHub Pages concluir com sucesso.
3. Se o site for publicado diretamente por branch, confira **Settings → Pages** para confirmar a origem.
4. Atualize `https://opusvix.github.io` usando `Ctrl + F5`.

### 2.6 Validar o portfólio

Confira em computador e celular:

- a imagem não está cortada de forma inadequada;
- o título aparece como **Porsche Enterprise Sales Intelligence**;
- a descrição está alinhada aos demais projetos;
- o botão GitHub abre `dashboard_porsche_sales`;
- o botão Dashboard abre a aplicação publicada;
- os links externos abrem sem erro;
- o novo projeto não quebrou a formatação dos itens seguintes.

---

## 3. Publicar no LinkedIn

### 3.1 Ordem recomendada

Publique no LinkedIn somente depois de concluir:

1. o repositório no GitHub;
2. a atualização do portfólio;
3. a validação dos três links.

Assim, nenhuma pessoa encontrará links ainda inexistentes.

### 3.2 Criar a publicação

1. Acesse `https://www.linkedin.com/feed/`.
2. Clique em **Começar publicação**.
3. Abra `docs/LINKEDIN_POST.md`.
4. Copie apenas o texto abaixo do título **Post para o LinkedIn**.
5. Cole no campo da publicação.
6. Confira se os três endereços aparecem completos:
   - dashboard;
   - GitHub;
   - portfólio.
7. Clique no ícone de imagem.
8. Envie `assets/dashboard-porsche-sales-cover.png`.
9. Adicione o texto alternativo:

   ```text
   Capa do dashboard Porsche Enterprise Sales Intelligence com visual executivo em preto e dourado e elementos de análise de dados.
   ```

10. Revise a quebra de linhas e publique.

### 3.3 Verificação após publicar

Depois da publicação:

1. Abra o post em uma nova guia.
2. Teste os três links.
3. Confirme que a imagem aparece em boa resolução.
4. Verifique se o trecho sobre a colaboração com ChatGPT/Codex está visível e claro.
5. Revise o aviso de projeto independente e sem vínculo oficial com a Porsche AG.

### 3.4 Destacar no perfil

Para aumentar a visibilidade profissional:

1. Abra seu perfil do LinkedIn.
2. Localize a seção **Destaques**.
3. Se ela ainda não existir, clique em **Adicionar seção do perfil → Recomendado → Adicionar aos Destaques**.
4. Adicione o post recém-publicado.
5. Reordene o item para colocá-lo entre os primeiros trabalhos exibidos.

Você também pode adicionar diretamente o link do dashboard ou do repositório como mídia destacada, mas destacar o post tende a apresentar melhor o contexto do projeto e da colaboração com IA.

---

## 4. Checklist final

### GitHub

- [ ] Repositório público criado com o nome correto.
- [ ] README e capa carregados.
- [ ] Link do dashboard funcionando.
- [ ] About, Website e Topics configurados.
- [ ] Declaração de desenvolvimento assistido por IA visível.

### Portfólio

- [ ] Imagem enviada para `assets`.
- [ ] Projeto inserido em **Projetos em Destaque**.
- [ ] Links de GitHub e Dashboard corretos.
- [ ] Publicação do GitHub Pages concluída.
- [ ] Layout validado em computador e celular.

### LinkedIn

- [ ] GitHub e portfólio publicados antes do post.
- [ ] Texto revisado.
- [ ] Capa anexada com texto alternativo.
- [ ] Colaboração com ChatGPT/Codex declarada.
- [ ] Post publicado e adicionado à seção Destaques.

---

## 5. Links finais

- Dashboard: `https://opusvix.github.io/dashboard_porsche_sales/`
- Repositório: `https://github.com/opusvix/dashboard_porsche_sales`
- Portfólio: `https://opusvix.github.io`
- LinkedIn: `https://www.linkedin.com/in/mauriciodasilvabarros/`

## Referências oficiais

- [Criar um repositório no GitHub](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)
- [Adicionar código local ao GitHub](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github)
- [Configurar a origem de publicação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Compartilhar links em uma publicação do LinkedIn](https://www.linkedin.com/help/linkedin/answer/a525301)
- [Gerenciar trabalhos na seção Destaques do LinkedIn](https://www.linkedin.com/help/linkedin/answer/a550399/manage-featured-samples-of-your-work-on-your-linkedin-profile)

