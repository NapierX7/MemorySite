# 🎁 Presente Romântico - Configuração e Uso

## 📋 Sobre o Projeto

Este é um sistema completo para criar presentes românticos personalizados com integração de pagamento via Mercado Pago e WhatsApp.

## 🚀 Arquivos do Projeto

### 1. `index.html` - Sistema Completo
- Sistema de preview para clientes testarem
- Demonstrações dos planos Básico e Premium
- Integração com Mercado Pago para pagamentos PIX
- Envio automático para WhatsApp após pagamento
- Layout romântico com corações flutuantes

### 2. `projeto-base.html` - Template para Clientes
- Arquivo limpo para personalizar para cada cliente
- Estrutura pronta para configurar dados do casal
- Layout idêntico ao sistema principal

## ⚙️ Configuração da API do Mercado Pago

### Passo 1: Criar Conta no Mercado Pago
1. Acesse [developers.mercadopago.com](https://developers.mercadopago.com)
2. Crie uma conta de desenvolvedor
3. Crie uma aplicação

### Passo 2: Obter Credenciais
1. No painel do desenvolvedor, vá em "Credenciais"
2. Copie o **Access Token** de teste ou produção
3. Substitua `TEST-YOUR-ACCESS-TOKEN` no código

### Passo 3: Configurar Webhook (Opcional)
1. Configure uma URL para receber notificações de pagamento
2. Substitua `https://seu-webhook.com/mercadopago` pela sua URL

## 🛠️ Como Usar o Projeto Base

### Para cada cliente, edite o arquivo `projeto-base.html`:

```javascript
// Encontre esta seção no código e configure:
const dadosPresente = {
    titulo: "Para Maria ♥", // Nome da pessoa especial
    fraseIntro: "João preparou algo especial para você ♥",
    nomeRemetente: "João", // Quem está dando o presente
    nomeDestinatario: "Maria", // Quem vai receber
    historia: "Nossa história começou em 2020...", // História do casal
    imagem: "foto-casal.jpg", // Caminho da foto
    dataInicio: "2020-03-15", // Data início do relacionamento
    spotifyLink: "https://open.spotify.com/track/..." // Link do Spotify
};
```

### Passos para Personalização:

1. **Copie o arquivo base**
   ```
   projeto-base.html → nome-do-cliente.html
   ```

2. **Configure os dados do casal**
   - Edite o objeto `dadosPresente`
   - Adicione a foto do casal na mesma pasta
   - Configure a data de início do relacionamento

3. **Teste o resultado**
   - Abra o arquivo no navegador
   - Clique em "Acessar" para ver o resultado

## 💰 Preços dos Planos

### Plano Básico - R$ 14,90
- Página personalizada
- Timer do relacionamento
- História do casal
- Layout romântico

### Plano Premium - R$ 24,90
- Tudo do Básico +
- Foto do casal
- Música especial do Spotify
- Corações flutuantes

## 📱 Integração WhatsApp

Após o pagamento aprovado, o sistema:
1. Envia automaticamente uma mensagem para o WhatsApp configurado
2. Inclui os detalhes do pagamento
3. Facilita o contato para entrega do produto

**Número configurado:** +55 61 98235-2620

## 🎨 Recursos Visuais

- **Fonte:** Dancing Script (romântica)
- **Cores:** Gradiente roxo/azul romântico
- **Animações:** Corações flutuantes
- **Layout:** Responsivo para mobile
- **Efeitos:** Hover nos botões, transições suaves

## 🔧 Personalização Avançada

### Alterar Cores
Edite as variáveis CSS no início do arquivo:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Alterar Preços
Edite a função `generatePaymentData`:
```javascript
const plans = {
    'basico': { price: 14.90, title: 'Plano Básico' },
    'premium': { price: 24.90, title: 'Plano Premium' }
};
```

### Adicionar Novos Planos
1. Adicione o plano na seção HTML
2. Configure o preço na função de pagamento
3. Adicione a demonstração se necessário

## 🚨 Importante

- **Teste sempre** com credenciais de teste antes de usar em produção
- **Configure o webhook** para receber notificações de pagamento
- **Mantenha as credenciais seguras** - nunca compartilhe publicamente
- **Teste em diferentes dispositivos** para garantir responsividade

## 📞 Suporte

Para dúvidas sobre configuração ou uso:
- WhatsApp: +55 61 98235-2620
- Email: suporte@presentesromanticos.com

---

**Desenvolvido com ♥ para criar momentos especiais**