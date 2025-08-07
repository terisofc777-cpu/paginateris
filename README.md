# Teris | Subliminares

Site profissional para canal Teris com sistema de administração completo.

## 🚀 Funcionalidades

- **PDFs Dinâmicos**: Lista de PDFs carregada automaticamente do arquivo `pdfs.json`
- **Sistema de Tradução**: Português, Inglês e Espanhol
- **Pedidos**: Formulários para pedidos gratuitos e personalizados
- **Feedback**: Sistema de comentários dos usuários
- **Painel Administrativo**: Controle de pedidos e mensagens
- **Netlify CMS**: Painel de administração global (visível para todos)

## 🎨 Design

- **Tema**: Vermelho com branco e dourado
- **Responsivo**: Funciona em todos os dispositivos
- **Animações**: Efeitos suaves e profissionais
- **Glassmorphism**: Design moderno com efeitos de vidro

## 📁 Estrutura dos Arquivos

```
temploteris/
├── index.html              # Site principal
├── pdfs.json              # Lista de PDFs (global)
├── customization.json     # Personalizações (global)
├── admin/
│   ├── index.html         # Painel Netlify CMS
│   └── config.yml         # Configuração do CMS
└── README.md              # Este arquivo
```

## 🔧 Como Usar

### Para Usuários Comuns
1. Acesse o site normalmente
2. Veja os PDFs disponíveis
3. Faça pedidos gratuitos ou personalizados
4. Deixe feedback

### Para Administradores

#### Painel Local (apenas no seu navegador)
1. Clique em "Login Administrador" no site
2. Controle pedidos e mensagens
3. **⚠️ Alterações são apenas locais**

#### Painel Global (Netlify CMS - visível para todos)
1. Acesse `/admin/` no seu site
2. Faça login com sua conta do GitHub
3. Edite PDFs e personalizações
4. **✅ Alterações ficam visíveis para todos**

## 🌐 Configuração no Netlify

### 1. Ativar Identity e Git Gateway
1. No painel do Netlify, vá em **Site settings** > **Identity**
2. Clique em **Enable Identity**
3. Vá em **Identity** > **Services** > **Git Gateway**
4. Clique em **Enable Git Gateway**

### 2. Configurar Usuários
1. Vá em **Identity** > **Users**
2. Clique em **Invite users**
3. Adicione seu email
4. Confirme o convite no email

### 3. Acessar o Painel ADM
1. Acesse `https://SEUSITE.netlify.app/admin/`
2. Faça login com sua conta do GitHub
3. Edite PDFs e personalizações

## 📝 Como Adicionar PDFs

### Via Netlify CMS (Recomendado)
1. Acesse `/admin/`
2. Vá em "PDFs"
3. Clique em "New PDF"
4. Preencha os campos:
   - **ID**: Número único
   - **Título**: Nome do PDF
   - **Link**: URL do arquivo PDF
   - **Idioma**: pt, en ou es
   - **Categoria**: manual, guide, tutorial ou other
   - **Data**: Data de adição (YYYY-MM-DD)
5. Clique em "Publish"

### Via Arquivo JSON (Manual)
Edite o arquivo `pdfs.json`:
```json
[
  {
    "id": 1,
    "title": "Nome do PDF",
    "link": "caminho/para/arquivo.pdf",
    "language": "pt",
    "category": "manual",
    "dateAdded": "2024-01-01"
  }
]
```

## 🎯 Personalizações

### Mensagem de Boas-vindas
Edite via Netlify CMS ou no arquivo `customization.json`:
```json
{
  "welcomeMessage": "Sua mensagem personalizada aqui",
  "siteTitle": "Título do Site"
}
```

## 🔄 Sistema de Tradução

O site suporta 3 idiomas:
- 🇧🇷 Português (padrão)
- 🇺🇸 Inglês
- 🇪🇸 Espanhol

Para adicionar traduções, edite o objeto `translations` no arquivo `index.html`.

## 🛠️ Tecnologias

- **HTML5**: Estrutura semântica
- **CSS3**: Design moderno com animações
- **JavaScript**: Funcionalidades dinâmicas
- **Netlify CMS**: Administração de conteúdo
- **GitHub Pages/Netlify**: Hospedagem

## 📞 Suporte

Para dúvidas ou problemas:
1. Verifique se o Identity e Git Gateway estão ativados no Netlify
2. Confirme se você está logado no painel ADM
3. Verifique se os arquivos JSON estão no formato correto

---

**Desenvolvido com ❤️ para o Canal Teris**


