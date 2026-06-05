# 📋 Instruções para publicar no GitHub Pages

## Passo 1: Criar repositório no GitHub

1. Acesse [github.com/new](https://github.com/new)
2. Crie um novo repositório com o nome: `logixsphere-manual`
3. Escolha "Public" (público)
4. Não marque "Initialize with README" (já temos um)
5. Clique em "Create repository"

## Passo 2: Adicionar o repositório remoto e fazer push

Execute os comandos abaixo (substitua USUARIO pelo seu nome de usuário do GitHub):

```bash
cd "/Users/mazinijoaomarcelo/Desktop/Pasta Sem Título"

git remote add origin https://github.com/USUARIO/logixsphere-manual.git
git branch -M main
git push -u origin main
```

## Passo 3: Configurar GitHub Pages

1. Vá até as configurações do repositório no GitHub
2. Na seção "Pages" (esquerda do menu)
3. Em "Build and deployment" → "Source", selecione "Deploy from a branch"
4. Em "Branch", selecione "main" e a pasta "/ (root)"
5. Clique em "Save"

## Passo 4: Aguarde o deploy

- Seu site estará disponível em: `https://USUARIO.github.io/logixsphere-manual/`
- Pode levar alguns minutos para publicar

## Passo 5 (Opcional): Configurar Domínio Customizado

Se você possui um domínio próprio e deseja usar em vez da URL padrão:

### No seu Registrador de Domínio:
1. Acesse as configurações DNS do seu domínio
2. Configure um registro CNAME apontando para `USUARIO.github.io`
   - Ou use registros A se preferir (veja documentação oficial)

### No GitHub:
1. Vá em Settings → Pages
2. Em "Custom domain", digite seu domínio (ex: `logixsphere.com`)
3. Marque "Enforce HTTPS" (recomendado)
4. Clique em "Save"

O GitHub Pages pode levar até 24 horas para validar o domínio.

---

**Dúvidas?** Veja a [documentação oficial do GitHub Pages](https://docs.github.com/en/pages) ou sobre [configuração de domínio customizado](https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site).
