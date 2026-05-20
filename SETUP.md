# 🚀 Guia de Configuração Rápida

## Passo 1: Adicionar o Logo

1. Salve o logo da empresa como `logo.png` na pasta `assets/`
2. O logo deve ter fundo transparente (formato PNG)
3. Dimensões recomendadas: 200x80px

## Passo 2: Testar o Site Localmente

### Opção 1: Abrir Diretamente no Navegador
```bash
# No macOS
open index.html

# No Windows
start index.html

# No Linux
xdg-open index.html
```

### Opção 2: Usar um Servidor Local (Recomendado)

**Com Python 3:**
```bash
python3 -m http.server 8000
```
Depois acesse: http://localhost:8000

**Com Node.js (npx):**
```bash
npx serve
```

**Com PHP:**
```bash
php -S localhost:8000
```

**Com VS Code:**
- Instale a extensão "Live Server"
- Clique com botão direito em `index.html`
- Selecione "Open with Live Server"

## Passo 3: Personalizar Conteúdo

### Alterar Informações de Contato
Edite o arquivo `index.html` e procure pela seção `<!-- Contato -->`

### Alterar Cores
Edite o arquivo `style.css` e modifique as variáveis CSS em `:root`

### Alterar Textos dos Banners
Edite o arquivo `index.html` na seção `<!-- Hero Section com Carrossel -->`

## Passo 4: Publicar Online

### GitHub Pages (Gratuito)
1. Crie um repositório no GitHub
2. Faça upload dos arquivos
3. Vá em Settings > Pages
4. Selecione a branch main
5. Seu site estará em: `https://seuusuario.github.io/nome-do-repo`

### Netlify (Gratuito)
1. Acesse https://netlify.com
2. Arraste a pasta do projeto
3. Site publicado instantaneamente!

### Vercel (Gratuito)
1. Acesse https://vercel.com
2. Importe o projeto
3. Deploy automático!

## 📋 Checklist de Verificação

- [ ] Logo adicionado em `assets/logo.png`
- [ ] Informações de contato atualizadas
- [ ] Textos dos banners personalizados
- [ ] Links do WhatsApp funcionando
- [ ] Link do Instagram correto
- [ ] Google Maps com localização correta
- [ ] Testado em dispositivos móveis
- [ ] Testado em diferentes navegadores

## 🔧 Solução de Problemas

### Logo não aparece
- Verifique se o arquivo está em `assets/logo.png`
- Verifique se o nome está correto (minúsculas)
- Limpe o cache do navegador (Ctrl+F5)

### Carrossel não funciona
- Verifique se o arquivo `script.js` está carregando
- Abra o Console do navegador (F12) para ver erros

### Menu mobile não abre
- Verifique se o JavaScript está habilitado
- Teste em outro navegador

### Animações não funcionam
- Alguns navegadores antigos podem não suportar
- Atualize para a versão mais recente do navegador

## 📱 Testar Responsividade

### No Navegador
1. Pressione F12 para abrir DevTools
2. Clique no ícone de dispositivo móvel
3. Teste diferentes tamanhos de tela

### Dispositivos Reais
- Teste em smartphone real
- Teste em tablet real
- Verifique orientação portrait e landscape

## 🎨 Customizações Avançadas

### Adicionar Mais Serviços
Copie um card de serviço existente em `index.html` e modifique o conteúdo.

### Mudar Velocidade do Carrossel
No arquivo `script.js`, procure por:
```javascript
autoPlayInterval = setInterval(nextSlide, 5000);
```
Altere `5000` para o valor desejado em milissegundos.

### Adicionar Mais Slides
1. Copie um `carousel-item` existente
2. Adicione um novo `indicator`
3. Atualize o JavaScript se necessário

## 📞 Suporte

Para dúvidas ou problemas:
- Verifique o arquivo README.md
- Consulte a documentação inline nos arquivos
- Revise os comentários no código

---

**Boa sorte com seu novo site! 🚀**