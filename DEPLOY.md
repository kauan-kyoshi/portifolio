# Deploy - Vercel (Gratuito e Profissional)

## Passo 1: Prepare o repositório GitHub

1. **Crie um repositório no GitHub:**
   - Acesse: https://github.com/new
   - Nome: `portifolio` (ou outro nome)
   - Privacidade: Público ou Privado (ambos funcionam)
   - **NÃO** inicialize com README

2. **Suba o código:**
   ```bash
   cd /home/kyoshi/Documentos/portifolio
   git init
   git add .
   git commit -m "Initial commit: Portfolio with Astro"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/portifolio.git
   git push -u origin main
   ```

## Passo 2: Deploy na Vercel

1. **Acesse:** https://vercel.com/signup
2. **Login com GitHub** (recomendado)
3. **Import Project:**
   - Clique em "Add New..." → "Project"
   - Selecione seu repositório `portifolio`
4. **Configure (auto-detecta Astro):**
   - Framework Preset: **Astro**
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`
5. **Deploy!** ✅

**Pronto em ~2 minutos!**

## URLs após deploy

- **Production:** `https://seu-nome.vercel.app`
- **Preview:** cada commit gera preview automático

## Atualizações futuras

Basta fazer push no GitHub:
```bash
git add .
git commit -m "Update: descrição da mudança"
git push
```

Vercel faz deploy automático em ~1 min.

## Domínio personalizado (opcional - GRÁTIS)

Se você tem um domínio (ex: `kauankyoshi.com`):
1. Vercel → Settings → Domains
2. Adicione seu domínio
3. Configure DNS (Vercel dá instruções)

---

## Alternativa: Netlify

Se preferir Netlify:
1. https://app.netlify.com/signup
2. "Add new site" → "Import from Git"
3. Selecione repositório
4. Build: `npm run build`, Publish: `dist`

---

## Checklist antes do deploy

- [ ] Atualize `src/data/projects.json` com seus repos reais
- [ ] Adicione sua foto em `public/profile.jpg`
- [ ] Teste local: `npm run build && npm run preview`
- [ ] Verifique que não há erros no console

## Performance esperada

- Lighthouse: 90-100 em todas métricas
- First Load: < 1s
- SEO: 100
