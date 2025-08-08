# 🔄 Instruções de Sincronização - Site Teris

## 🎯 Como Funciona a Sincronização

### **Sistema de Arquivo Compartilhado**
O site agora usa um arquivo `admin-settings.json` que é compartilhado entre todos os dispositivos. Quando o admin faz mudanças, elas são salvas neste arquivo e todos os dispositivos leem as mudanças automaticamente.

## 📋 Como Atualizar as Configurações

### **1. Fazer Mudanças como Admin**
1. **Faça login como admin** no site
2. **Clique nos botões** para fazer as mudanças desejadas
3. **Clique em "📋 Ver Configurações Atuais"** no painel admin
4. **Copie o texto** que aparece na janela

### **2. Atualizar o Arquivo admin-settings.json**
1. **Abra o arquivo** `admin-settings.json` no seu editor
2. **Substitua todo o conteúdo** pelo texto copiado
3. **Salve o arquivo**
4. **Faça upload** do arquivo atualizado para o servidor

### **3. Verificar Sincronização**
- **Aguarde 2-3 segundos** para que os dispositivos detectem a mudança
- **Verifique** se as mudanças aparecem em outros dispositivos
- **Use o botão "🔄 Sincronizar"** em dispositivos móveis se necessário

## 🔧 Exemplo de Arquivo admin-settings.json

```json
{
  "freeOrdersEnabled": false,
  "customOrdersEnabled": true,
  "feedbackEnabled": true,
  "pdfsEnabled": false,
  "lastUpdate": "2024-01-15T14:30:00.000Z",
  "version": "1.0"
}
```

## 📱 Configurações Disponíveis

### **freeOrdersEnabled**
- `true`: Pedidos gratuitos habilitados
- `false`: Pedidos gratuitos desabilitados

### **customOrdersEnabled**
- `true`: Encomendas personalizadas habilitadas
- `false`: Encomendas personalizadas desabilitadas

### **feedbackEnabled**
- `true`: Seção de feedback visível
- `false`: Seção de feedback oculta

### **pdfsEnabled**
- `true`: Seção de PDFs visível
- `false`: Seção de PDFs oculta

### **lastUpdate**
- Timestamp da última atualização (atualizado automaticamente)

### **version**
- Versão do sistema (não alterar)

## 🚀 Processo Completo

### **Cenário: Desabilitar Pedidos Gratuitos**

1. **Admin no PC**:
   - Faz login como admin
   - Clica em "Aceitar/Rejeitar Pedidos Gratuitos"
   - Status muda para "⚠️ Aceitando Pedidos Parcialmente"
   - Clica em "📋 Ver Configurações Atuais"
   - Copia o texto mostrado

2. **Atualizar Arquivo**:
   - Abre `admin-settings.json`
   - Substitui o conteúdo pelo texto copiado
   - Salva e faz upload

3. **Verificar Sincronização**:
   - Aguarda 2-3 segundos
   - Verifica se outros dispositivos atualizaram
   - Usa "🔄 Sincronizar" se necessário

## 🔍 Verificações Importantes

### **Antes de Fazer Upload**
- [ ] Arquivo JSON está válido
- [ ] Todas as configurações estão presentes
- [ ] `lastUpdate` foi atualizado
- [ ] `version` permanece "1.0"

### **Após o Upload**
- [ ] Arquivo está acessível via URL
- [ ] Dispositivos detectam a mudança
- [ ] Interface atualiza corretamente
- [ ] Notificações aparecem

## 🐛 Solução de Problemas

### **Mudanças não aparecem**
1. **Verifique se o arquivo foi salvo corretamente**
2. **Confirme se o upload foi bem-sucedido**
3. **Teste o botão "🔄 Sincronizar"**
4. **Verifique se não há erros no console**

### **Arquivo não encontrado**
1. **Confirme se o arquivo está no local correto**
2. **Verifique as permissões do arquivo**
3. **Teste o acesso direto à URL**
4. **Use localStorage como fallback**

### **Sincronização lenta**
1. **Verifique a conexão com a internet**
2. **Confirme se o cache está sendo limpo**
3. **Teste com diferentes intervalos**
4. **Use o botão de sincronização manual**

## ✅ Checklist de Sincronização

### **Antes de Fazer Mudanças**
- [ ] Backup do arquivo atual
- [ ] Verificação de permissões
- [ ] Teste de acesso ao arquivo

### **Durante as Mudanças**
- [ ] Mudanças aplicadas corretamente
- [ ] Configurações copiadas
- [ ] Arquivo atualizado

### **Após as Mudanças**
- [ ] Arquivo salvo e enviado
- [ ] Sincronização verificada
- [ ] Dispositivos atualizados
- [ ] Funcionalidade testada

---

**🎉 Com estas instruções, a sincronização entre dispositivos funcionará perfeitamente!**

## 🚀 Status Final

**✅ Sistema de Sincronização Completo:**
- **Arquivo Compartilhado**: admin-settings.json
- **Processo Manual**: Admin atualiza o arquivo
- **Detecção Automática**: Dispositivos leem mudanças
- **Fallback**: localStorage como backup
- **Botão Manual**: Sincronização forçada
- **Logs Detalhados**: Debug completo

**A sincronização está agora completamente funcional!** 🔄
