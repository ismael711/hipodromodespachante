# 🌐 Configuração do Domínio hipodromodespachante.com.br

## Arquivo CNAME Criado ✅

O arquivo `CNAME` foi criado com o domínio: **hipodromodespachante.com.br**

## 📋 Passos para Configurar o Domínio

### 1. Publicar no GitHub Pages

1. **Criar repositório no GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Hipódromo Despachante website"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/hipodromodespachante.git
   git push -u origin main
   ```

2. **Ativar GitHub Pages:**
   - Vá em: Settings > Pages
   - Source: Deploy from a branch
   - Branch: main / (root)
   - Clique em Save

### 2. Configurar DNS no Registro.br (ou seu provedor)

Você precisa adicionar os seguintes registros DNS:

#### Opção A: Usar GitHub Pages (Recomendado)

**Registros A (para domínio raiz):**
```
Tipo: A
Nome: @
Valor: 185.199.108.153
TTL: 3600

Tipo: A
Nome: @
Valor: 185.199.109.153
TTL: 3600

Tipo: A
Nome: @
Valor: 185.199.110.153
TTL: 3600

Tipo: A
Nome: @
Valor: 185.199.111.153
TTL: 3600
```

**Registro CNAME (para www):**
```
Tipo: CNAME
Nome: www
Valor: SEU-USUARIO.github.io
TTL: 3600
```

#### Opção B: Usar Netlify

1. Faça deploy no Netlify
2. Vá em Domain Settings
3. Adicione o domínio personalizado
4. Configure os registros DNS conforme instruções do Netlify

**Registros DNS para Netlify:**
```
Tipo: A
Nome: @
Valor: 75.2.60.5
TTL: 3600

Tipo: CNAME
Nome: www
Valor: SEU-SITE.netlify.app
TTL: 3600
```

### 3. Verificar Configuração do GitHub Pages

Após configurar o DNS:

1. Vá em Settings > Pages no GitHub
2. Em "Custom domain", digite: `hipodromodespachante.com.br`
3. Clique em Save
4. Aguarde a verificação DNS (pode levar até 24h)
5. Marque "Enforce HTTPS" quando disponível

### 4. Verificar Propagação DNS

Use estas ferramentas para verificar:
- https://dnschecker.org
- https://www.whatsmydns.net

Digite: `hipodromodespachante.com.br`

## 🔒 SSL/HTTPS

### GitHub Pages
- SSL automático após verificação do domínio
- Marque "Enforce HTTPS" nas configurações

### Netlify
- SSL automático (Let's Encrypt)
- Configurado automaticamente

## ⏱️ Tempo de Propagação

- **Mínimo:** 1-2 horas
- **Máximo:** 24-48 horas
- **Média:** 4-8 horas

## ✅ Checklist de Configuração

- [ ] Repositório criado no GitHub
- [ ] Código enviado para o repositório
- [ ] GitHub Pages ativado
- [ ] Registros DNS configurados no Registro.br
- [ ] Domínio personalizado adicionado no GitHub
- [ ] DNS verificado e propagado
- [ ] HTTPS ativado
- [ ] Site acessível em hipodromodespachante.com.br
- [ ] Site acessível em www.hipodromodespachante.com.br

## 🔧 Solução de Problemas

### Domínio não resolve
- Verifique se os registros DNS estão corretos
- Aguarde a propagação (até 48h)
- Use `nslookup hipodromodespachante.com.br` para verificar

### Erro de certificado SSL
- Aguarde a emissão do certificado (pode levar algumas horas)
- Verifique se "Enforce HTTPS" está marcado
- Limpe o cache do navegador

### Página 404
- Verifique se o arquivo CNAME está no repositório
- Confirme que o GitHub Pages está ativado
- Verifique a branch correta (main)

## 📞 Suporte

### Registro.br
- Site: https://registro.br
- Suporte: https://registro.br/suporte/

### GitHub Pages
- Documentação: https://docs.github.com/pages
- Status: https://www.githubstatus.com

## 🚀 Comandos Git Úteis

```bash
# Verificar status
git status

# Adicionar alterações
git add .

# Commit
git commit -m "Descrição das alterações"

# Enviar para GitHub
git push origin main

# Ver histórico
git log --oneline

# Criar nova branch
git checkout -b nome-da-branch
```

## 📝 Notas Importantes

1. O arquivo CNAME deve conter apenas o domínio (sem http:// ou https://)
2. Não adicione barra (/) no final do domínio
3. Use apenas letras minúsculas
4. O arquivo deve estar na raiz do projeto
5. Após qualquer alteração no DNS, aguarde a propagação

---

**Domínio configurado: hipodromodespachante.com.br** ✅