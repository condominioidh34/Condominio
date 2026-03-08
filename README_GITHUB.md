# CondoPro Cloud Edition ☁️

**Sistema de Gestão de Condomínios 100% na Cloud**

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-blue?logo=github)](https://pages.github.com/)
[![Google Drive](https://img.shields.io/badge/Google-Drive-green?logo=google-drive)](https://drive.google.com/)
[![License](https://img.shields.io/badge/License-Free-success)](LICENSE)

---

## 🎯 O Que É?

CondoPro Cloud Edition é um sistema **completo e gratuito** para gerir condomínios, com:

- ✅ **Dados 100% na Google Drive** - Seguro, sincronizado, acessível
- ✅ **Acesso Multi-Utilizador** - Todos trabalham nos mesmos dados
- ✅ **Sistema de Votações Completo** - Actas digitais com resultados automáticos
- ✅ **Gestão Financeira** - Quotas, pagamentos, recibos
- ✅ **Ocorrências** - Registo e acompanhamento
- ✅ **0€ Custos** - Sem servidor, sem mensalidades

---

## 🚀 Instalação Rápida (5 minutos)

### 1. Configurar Google Drive API

1. Vai a [Google Cloud Console](https://console.cloud.google.com/)
2. Cria projeto "CondoPro"
3. Ativa Google Drive API
4. Cria credenciais OAuth 2.0
5. Guarda o **Client ID**

📖 **[Ver Guia Completo →](SETUP_GITHUB.md)**

### 2. Publicar no GitHub Pages

1. Faz fork/clone deste repositório
2. Edita `index.html` e cola o teu Client ID:
   ```javascript
   GOOGLE_CLIENT_ID: 'o-teu-client-id.apps.googleusercontent.com',
   ```
3. Settings → Pages → Ativa GitHub Pages
4. Pronto! Acede a `https://teu-username.github.io/condopro/`

---

## 📱 Como Funciona

```
┌─────────────────────────────────────┐
│   GitHub Pages (Hosting Grátis)    │
│   https://username.github.io        │
│                                     │
│   Interface Web                     │
└──────────────┬──────────────────────┘
               │
               │ Read/Write
               ▼
┌─────────────────────────────────────┐
│   Google Drive (Base de Dados)     │
│   📁 CondoPro_Data/                 │
│      ├─ state.json                  │
│      └─ backups/                    │
└─────────────────────────────────────┘
               ▲
               │
               │ Sync (30s)
               │
┌──────────┬──────────┬──────────┐
│ Admin    │ Condó 1  │ Condó 2  │
│ Desktop  │ Mobile   │ Tablet   │
└──────────┴──────────┴──────────┘
```

**Todos acedem aos mesmos dados em tempo real!**

---

## ✨ Funcionalidades

### 📊 Dashboard
- Estatísticas financeiras
- Resumo de pagamentos
- Próximas reuniões

### 👥 Gestão de Condóminos
- Cadastro completo
- Frações e quotas
- Ativo/Inativo

### 💰 Financeiro
- Quotas mensais
- Pagamentos e recibos
- Histórico completo

### 🗳️ Actas e Votações
- Criar reuniões
- Pontos de votação individuais
- Sistema de votos: A Favor / Contra / Abstenção
- Cálculo automático de quórum
- Geração automática de ata final
- Resultados em tempo real

### 📝 Ocorrências
- Registo de problemas
- Acompanhamento de estado
- Respostas da administração

### ⚙️ Definições
- Dados do condomínio
- Logo personalizado
- Rodapé de recibos

---

## 🎮 Demo

**URL de Exemplo**: https://username.github.io/condopro/

**Login Inicial**:
- Email: `admin@condopro.pt`
- Password: `admin123`

⚠️ **Muda a password nas definições!**

---

## 📖 Documentação

- **[Guia de Instalação Completo](SETUP_GITHUB.md)** - Passo-a-passo detalhado
- **[FAQ](FAQ.md)** - Perguntas frequentes
- **[Troubleshooting](TROUBLESHOOTING.md)** - Resolução de problemas

---

## 🔒 Segurança

- ✅ **HTTPS** obrigatório (GitHub Pages)
- ✅ **OAuth 2.0** do Google
- ✅ **Dados privados** - Cada utilizador tem os seus dados no seu Google Drive
- ✅ **Sem servidor intermédio** - Dados nunca passam por terceiros
- ✅ **Código open-source** - Podes auditar tudo

---

## 💻 Requisitos

- Navegador moderno (Chrome, Firefox, Safari, Edge)
- Conta Google (grátis)
- Conta GitHub (grátis)

**Funciona em**:
- 💻 Desktop (Windows, Mac, Linux)
- 📱 Mobile (iOS, Android)
- 📱 Tablets

---

## 🆘 Suporte

### Problemas Comuns

**"Redirect URI mismatch"**
→ Verifica que o URI OAuth é exatamente: `https://username.github.io`

**"Access Blocked"**
→ Adiciona o teu email em OAuth consent screen → Test users

**"Dados não sincronizam"**
→ Faz refresh (F5). Sincronização automática a cada 30s.

📖 [Ver mais em Troubleshooting](TROUBLESHOOTING.md)

---

## 🗺️ Roadmap

- [ ] App mobile nativa (iOS/Android)
- [ ] Notificações push
- [ ] Chat entre condóminos
- [ ] Export PDF de actas
- [ ] Calendário integrado
- [ ] Multi-condomínio (gerir vários prédios)

---

## 🤝 Contribuir

Contribuições são bem-vindas!

1. Fork este repositório
2. Cria uma branch: `git checkout -b nova-funcionalidade`
3. Commit: `git commit -am 'Adiciona nova funcionalidade'`
4. Push: `git push origin nova-funcionalidade`
5. Abre um Pull Request

---

## 📄 Licença

Software livre para uso em condomínios.  
Usa, modifica e distribui à vontade.

---

## 🌟 Créditos

Desenvolvido com ❤️ para facilitar a gestão de condomínios.

**Tecnologias**:
- HTML5 + CSS3 + Vanilla JavaScript
- Google Drive API
- GitHub Pages
- IndexedDB (cache local)

---

## 📞 Contacto

Problemas? Sugestões?

- 📧 Email: [teu-email@exemplo.com]
- 🐛 Issues: [GitHub Issues](../../issues)
- 💬 Discussões: [GitHub Discussions](../../discussions)

---

**⭐ Se achaste útil, dá uma estrela no GitHub!**

---

**Versão**: 2.0 Cloud Edition  
**Última atualização**: Março 2026  
**Status**: ✅ Produção
