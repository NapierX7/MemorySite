# 💕 Presentes Românticos - Versão Simplificada

## 🎯 Objetivo
Este é um projeto **simplificado** para gerar renda rapidamente com presentes românticos personalizados, sem as complexidades técnicas do projeto original.

## ✨ Como Funciona

### Para o Cliente:
1. Acessa o site
2. Preenche o formulário com:
   - Nome da pessoa especial
   - Mensagem de amor
   - Foto (opcional)
   - Link do Spotify (opcional)
   - Seus dados de contato
3. Vê um preview do presente
4. Escolhe um plano e clica em "Comprar via WhatsApp"
5. É redirecionado para seu WhatsApp com todos os dados

### Para Você (Vendedor):
1. Recebe a mensagem no WhatsApp com todos os dados
2. Confirma o pagamento (PIX, transferência, etc.)
3. Cria o presente manualmente usando os dados recebidos
4. Envia o link do presente para o cliente

## 💰 Planos de Preço
- **Básico**: R$ 19,90 - Presente simples
- **Premium**: R$ 34,90 - Com extras românticos

## 🚀 Como Usar

### 1. Configurar seu WhatsApp
No arquivo `index.html`, linha 340, altere o número:
```javascript
const whatsappUrl = `https://wa.me/61982352620?text=${encodeURIComponent(message)}`;
```

### 2. Hospedar o Site
Opções gratuitas:
- **Netlify**: Arraste a pasta para netlify.com
- **Vercel**: Conecte com GitHub
- **GitHub Pages**: Suba para um repositório público

### 3. Processo de Venda
1. Cliente preenche e escolhe plano
2. Você recebe no WhatsApp
3. Confirma pagamento
4. Cria o presente usando o projeto original como base
5. Entrega o link

## 🎨 Criando os Presentes
Use o projeto original (`Romantico/`) como ferramenta para criar os presentes:
1. Use os dados recebidos no WhatsApp
2. Crie o presente no projeto original
3. Gere o link
4. Envie para o cliente

## 💡 Vantagens desta Versão
- ✅ **Zero complexidade técnica**
- ✅ **Sem servidor necessário**
- ✅ **Sem banco de dados**
- ✅ **Sem APIs de pagamento**
- ✅ **Funciona imediatamente**
- ✅ **Você controla todo o processo**
- ✅ **Sem bugs ou problemas técnicos**

## 📈 Estratégia de Crescimento
1. **Fase 1**: Use esta versão para validar o mercado
2. **Fase 2**: Quando tiver clientes regulares, volte ao projeto automatizado
3. **Fase 3**: Reinvista os lucros em melhorias técnicas

## 🔧 Personalização
- Altere cores no CSS (variáveis no `:root`)
- Modifique textos e preços
- Adicione/remova campos do formulário
- Personalize as mensagens do WhatsApp

## 📱 Responsivo
O site funciona perfeitamente em celulares e tablets.

---

**💪 Comece hoje mesmo e valide sua ideia de negócio!**