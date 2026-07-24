# Site — GM Delavechia / ASAMCO Martial Arts

## Estrutura de arquivos

```
site/
├── index.html              → página principal (home)
├── style.css                → estilo visual do site inteiro
└── blog/
    ├── 30-anos-asamco.html
    ├── mma-cientifica.html
    └── formando-faixas-pretas.html
```

Tudo que está entre `[colchetes]` ainda precisa ser preenchido com conteúdo real
(foto, e-mail, WhatsApp, textos dos artigos, links de redes sociais).

## Como publicar no GitHub Pages (passo a passo)

### 1. Criar uma conta no GitHub (se ainda não tiver)
Acesse https://github.com e crie uma conta gratuita.

### 2. Criar um novo repositório
- Clique em **New repository**
- Nome sugerido: `gm-delavechia` (pode ser outro)
- Deixe como **Public**
- Não marque "Add a README" (já temos um)
- Clique em **Create repository**

### 3. Subir os arquivos
Na página do repositório recém-criado:
- Clique em **uploading an existing file**
- Arraste TODOS os arquivos desta pasta (`index.html`, `style.css`, a pasta `blog/` inteira e este `README.md`)
- Escreva uma mensagem como "primeiro upload do site" e clique em **Commit changes**

*(Se preferir usar Git pela linha de comando, os comandos seriam:)*
```bash
git init
git add .
git commit -m "primeiro upload do site"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/gm-delavechia.git
git push -u origin main
```

### 4. Ativar o GitHub Pages
- No repositório, vá em **Settings** (aba no topo)
- No menu lateral, clique em **Pages**
- Em "Source", selecione a branch **main** e a pasta **/ (root)**
- Clique em **Save**

### 5. Acessar o site no ar
Depois de alguns minutos, o GitHub vai gerar um link no formato:
```
https://SEU-USUARIO.github.io/gm-delavechia/
```
Esse é o endereço público do seu site.

## Como publicar um novo artigo no futuro

1. Peça para eu criar o arquivo HTML do novo artigo (mesmo padrão visual dos outros)
2. Coloque o arquivo dentro da pasta `blog/`
3. Adicione um novo card em `index.html`, na seção `<div class="blog-grid">`, linkando para o novo arquivo
4. Suba os arquivos atualizados no GitHub (upload manual ou `git push`)

## Domínio próprio (opcional, mais profissional)

Depois que o site estiver no ar em `github.io`, é possível apontar um domínio
próprio (ex: `gmdelavechia.com.br`) para ele, configurando um CNAME nas
configurações de DNS do domínio e no GitHub Pages. Posso te ajudar com isso
quando chegar a hora.
