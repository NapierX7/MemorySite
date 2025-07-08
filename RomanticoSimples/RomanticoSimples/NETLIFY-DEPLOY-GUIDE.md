# 🚀 Guia de Deploy no Netlify - Troubleshooting

## ✅ Arquivos Criados para Resolver Problemas

### 1. `netlify.toml` - Configuração Principal
- Configurações de build e redirecionamentos
- Headers de segurança
- Cache para arquivos estáticos

### 2. `_redirects` - Redirecionamentos (Backup)
- Garante que todas as rotas apontem para index.html
- Funciona como fallback se o netlify.toml falhar

## 🔧 Problemas Comuns e Soluções

### Problema 1: Site não carrega após deploy
**Causa:** Caminhos de arquivos incorretos
**Solução:** ✅ Já resolvido com os arquivos de configuração

### Problema 2: Imagens não aparecem
**Causa:** Arquivos de imagem não foram enviados ou caminhos incorretos
**Soluções:**
1. Verifique se as imagens estão na pasta:
   - `Maduh.jpg`
   - `fotomaduh.jpg` 
   - `minha_foto.jpg`

2. Se as imagens não existem, substitua por placeholders:
```javascript
// No código, substitua:
imagem1: 'Maduh.jpg',
imagem2: 'fotomaduh.jpg', 
imagem3: 'minha_foto.jpg'

// Por:
imagem1: 'https://via.placeholder.com/300x200/ff6b9d/ffffff?text=Foto+1',
imagem2: 'https://via.placeholder.com/300x200/ff6b9d/ffffff?text=Foto+2',
imagem3: 'https://via.placeholder.com/300x200/ff6b9d/ffffff?text=Foto+3'
```

### Problema 3: Formulário não funciona
**Causa:** JavaScript bloqueado ou erro de console
**Soluções:**
1. Abra o console do navegador (F12)
2. Verifique se há erros relacionados a:
   - Imagens não encontradas
   - Funções JavaScript
   - CORS (Cross-Origin)

### Problema 4: WhatsApp não abre
**Causa:** Bloqueio de pop-ups ou URL malformada
**Solução:** ✅ Código já está correto

### Problema 5: Mercado Pago não funciona
**Causa:** Chaves de API inválidas ou ambiente de teste
**Soluções:**
1. Verifique se as chaves estão corretas
2. Use chaves de produção (não teste) para site público
3. Configure webhook se necessário

## 📋 Checklist de Deploy

### Antes do Deploy:
- [ ] Todas as imagens estão na pasta
- [ ] Número do WhatsApp está correto
- [ ] Chaves do Mercado Pago estão configuradas
- [ ] Site funciona localmente

### Durante o Deploy:
- [ ] Arraste TODA a pasta para o Netlify
- [ ] Inclua os arquivos: `netlify.toml` e `_redirects`
- [ ] Aguarde o build completar

### Após o Deploy:
- [ ] Teste o formulário
- [ ] Teste os botões de WhatsApp
- [ ] Teste as demonstrações
- [ ] Verifique se as imagens carregam
- [ ] Teste em mobile

## 🛠️ Como Fazer o Deploy Correto

### Método 1: Drag & Drop (Recomendado)
1. Acesse [netlify.com](https://netlify.com)
2. Faça login ou crie conta
3. Arraste a pasta `RomanticoSimples` inteira para a área de deploy
4. Aguarde o processo completar
5. Teste o site no link fornecido

### Método 2: GitHub (Avançado)
1. Suba o projeto para um repositório GitHub
2. Conecte o Netlify ao repositório
3. Configure build settings:
   - Build command: `echo 'No build needed'`
   - Publish directory: `.`

## 🚨 Erros Específicos e Soluções

### Erro: "Page Not Found"
**Solução:** ✅ Resolvido com `_redirects` e `netlify.toml`

### Erro: "Mixed Content" (HTTP/HTTPS)
**Solução:** Todas as URLs externas já usam HTTPS

### Erro: "Failed to load resource"
**Solução:** Verifique se todos os arquivos foram enviados

### Erro: Console JavaScript
**Solução:** Abra F12 e verifique erros específicos

## 📞 Suporte Adicional

Se ainda houver problemas:
1. Compartilhe o link do site no Netlify
2. Compartilhe prints dos erros no console (F12)
3. Descreva exatamente o que não está funcionando

## 🎯 Resultado Esperado

Após seguir este guia, seu site deve:
- ✅ Carregar completamente
- ✅ Mostrar todas as imagens
- ✅ Formulário funcionando
- ✅ Botões de WhatsApp funcionando
- ✅ Demonstrações funcionando
- ✅ Responsivo em mobile

---

**💡 Dica:** Sempre teste localmente antes de fazer deploy!