# 🔥 Churrasco Premium 2026

Um site elegante e responsivo para gerenciar confirmações de presença em um evento de churrasco exclusivo, com funcionalidades para convidados e administradores.

---

## 🎯 Funcionalidades

### Para Convidados 👥
- ✅ **Confirmação de Presença** - Informe quantos adultos e crianças irão
- 📅 **Countdown** - Acompanhe os dias, horas e minutos até o evento
- 🍖 **Cardápio** - Veja o menu completo organizado em categorias
- ⏰ **Cronograma** - Conheça a programação do dia
- 📍 **Localização** - Mapa integrado do local do evento
- 📸 **Galeria** - Fotos do evento com suporte a upload (admin)
- 📢 **Avisos** - Receba notícias importantes sobre o evento
- 💬 **Confirmar via WhatsApp** - Compartilhe sua confirmação no WhatsApp

### Para Administradores ⚙️
- 📋 **Lista de Confirmados** - Tabela completa com todos os convidados
- 🔲 **QR Codes** - Gere QR codes para cada convidado
- 📥 **Exportar para CSV** - Baixe a lista em Excel/CSV
- ➕ **Adicionar Convidados** - Insira manualmente convidados
- 📢 **Publicar Avisos** - Envie mensagens para todos os convidados
- 📸 **Gerenciar Galeria** - Upload e gerenciamento de fotos

---

## 🚀 Como Acessar

1. **Acesse o site** via GitHub Pages: https://erivelson82.github.io/Confirmar-Presen-a-/

2. **Credenciais de Acesso:**
   - **Convidado**: `bbq2026`
   - **Admin**: `admin2026`

---

## 📋 Eventos

**Evento:** Churrasco Premium 2026  
**Data:** 12 de Julho de 2026  
**Hora:** A partir das 13:00  
**Local:** Wind Residencial - Estr. dos Bandeirantes, 7700 - Jacarepaguá, Rio de Janeiro - RJ

---

## 🍽️ Cardápio

### 🥩 Carnes
- Picanha
- Fraldinha
- Linguiça
- Coração

### 🍗 Aves
- Asa de Frango
- Sobrecoxa

### 🥗 Acompanhamentos
- Arroz
- Farofa
- Vinagrete
- Pão de Alho

### 🥤 Bebidas
- Refrigerante
- Água
- Suco

### 🍰 Sobremesas
- Bolo
- Docinhos

---

## 💾 Tecnologia

- **HTML5** - Estrutura
- **CSS3** - Estilização responsiva
- **JavaScript Vanilla** - Funcionalidades interativas
- **LocalStorage** - Persistência de dados (no navegador)
- **Google Maps API** - Mapa integrado
- **QR Server API** - Geração de QR codes

---

## 🎨 Design

- 🌙 **Tema Escuro** - Interface elegante e moderna
- 📱 **Responsivo** - Otimizado para desktop, tablet e celular
- 🔥 **Cores Quentes** - Laranja e vermelho para tema de churrasco
- ⚡ **Rápido** - Sem dependências externas pesadas

---

## 📊 Dados

Todos os dados são armazenados **localmente no navegador** usando:
- `localStorage` para confirmações
- `localStorage` para avisos
- `localStorage` para galeria
- `localStorage` para cardápio personalizado

> **Nota:** Os dados não são enviados para servidores externos. Cada navegador/dispositivo tem seus próprios dados.

---

## 🔐 Segurança

⚠️ **Importante:**
- As senhas são apenas para demonstração
- Este é um site de cliente (frontend only)
- Para produção, implemente autenticação backend adequada
- Os dados são públicos para anyone com acesso à página

---

## 📱 Navegação

| Seção | Ícone | Descrição |
|-------|-------|-----------|
| Home | 🏠 | Página inicial com countdown |
| Cardápio | 🍖 | Menu do evento |
| Confirmar | ✅ | RSVP e preenchimento de dados |
| Cronograma | ⏰ | Timeline do evento |
| Local | 📍 | Mapa e direções |
| Galeria | 📸 | Fotos do evento |
| Avisos | 📢 | Mensagens importantes |
| Admin | ⚙️ | Painel administrativo (senha necessária) |

---

## 🛠️ Como Personalizar

### Alterar Data do Evento
Edite a linha no `index.html`:
```javascript
const EVENT_DATE = new Date('2026-07-12T13:00:00-03:00');
```

### Alterar Senhas
```javascript
const SENHA_CONVIDADO = 'bbq2026';
const SENHA_ADMIN = 'admin2026';
```

### Alterar Cardápio
```javascript
const cardapioPadrao = {
    carnes: [ /* itens */ ],
    // ...
};
```

### Alterar Localização
1. Acesse https://maps.google.com
2. Encontre seu local
3. Copie o embed URL
4. Substitua no `<iframe>` dentro de `#page-localizacao`

---

## 📞 Suporte

Se tiver dúvidas ou problemas:
1. Verifique se está usando a senha correta
2. Limpe o cache do navegador (Ctrl+Shift+Delete)
3. Tente em outro navegador
4. Verifique o console (F12) para mensagens de erro

---

## 📄 Licença

Este projeto é de uso livre. Sinta-se à vontade para clonar, modificar e usar em seus eventos!

---

## 👤 Desenvolvido por

**erivelson82** - GitHub: [@erivelson82](https://github.com/erivelson82)

---

## 🎉 Bom Churrasco!

Aproveite o evento e se divirta! 🥩🔥✨
