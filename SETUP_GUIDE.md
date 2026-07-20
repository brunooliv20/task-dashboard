# 🚀 Guia de Setup - Painel de Tarefas em Português

Bem-vindo! Este guia vai te ajudar a instalar e executar a aplicação **Painel de Tarefas** traduzida para português brasileiro.

---

## 📋 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- **Node.js** v18 ou superior ([Baixar](https://nodejs.org/))
- **npm** v10 ou superior (vem com Node.js)
- **Git** ([Baixar](https://git-scm.com/))

### Verificar Instalação

```bash
node --version    # Deve mostrar v18+
npm --version     # Deve mostrar v10+
git --version     # Deve mostrar a versão do git
```

---

## 🛠️ Instalação Passo a Passo

### 1️⃣ Clonar o Repositório

```bash
# Clone com a branch de tradução
git clone -b traducao-portugues-brasil https://github.com/brunooliv20/task-dashboard.git
cd task-dashboard
```

### 2️⃣ Instalar Dependências

```bash
npm install
```

Isso vai instalar todas as bibliotecas necessárias como React, Tailwind CSS e Framer Motion.

### 3️⃣ Iniciar o Servidor de Desenvolvimento

```bash
npm start
```

A aplicação abrirá automaticamente em [http://localhost:3000](http://localhost:3000).

---

## 💻 Usando a Aplicação

### Funcionalidades Principais

#### ➕ Adicionar Tarefa
1. Clique em **"Adicionar Nova Tarefa"**
2. Digite a descrição no campo: *"O que precisa ser feito?"*
3. Adicione tags (opcional) digitando no campo de tags
4. Clique no ✅ para criar

#### 🏷️ Gerenciar Tags
1. Clique em **"Gerenciar Tags"**
2. Adicione novas tags no campo
3. Edite ou delete tags existentes
4. As tags são automáticas para novas tarefas

#### 📋 Criar Listas Filtradas
1. Clique em **"Adicionar Nova Lista"**
2. Configure filtros (tags específicas, status de conclusão)
3. A lista será preenchida automaticamente com tarefas que correspondem aos filtros

#### ✅ Completar Tarefas
- Clique no checkbox próximo à tarefa
- Ou use **"Completar Tudo"** para completar todas as tarefas da lista

---

## 🧪 Scripts Disponíveis

```bash
# Iniciar desenvolvimento
npm start

# Build para produção
npm run build

# Preview do build de produção
npm run preview

# Executar testes
npm test

# Build com dados de demonstração
npm run build:hydrated

# Preview com dados de demonstração
npm run preview:hydrated
```

---

## 📊 Estrutura do Projeto

```
task-dashboard/
├── src/
│   ├── App.jsx                    # Componente principal
│   ├── features/
│   │   ├── tasks/                 # Componentes de tarefas
│   │   ├── lists/                 # Componentes de listas
│   │   └── tags/                  # Componentes de tags
│   ├── context/                   # Gerenciamento de estado
│   └── index.jsx                  # Entrada da aplicação
├── index.html                     # HTML principal (pt-BR)
├── README.md                      # Documentação em português
└── VALIDATION_REPORT.md          # Relatório de validação
```

---

## 🌍 Linguagem da Interface

A aplicação está **100% em português brasileiro (pt-BR)**:

- ✅ Títulos em português
- ✅ Placeholders traduzidos
- ✅ Botões em português
- ✅ Mensagens de feedback em português
- ✅ Documentação em português

---

## 🐛 Troubleshooting

### ❌ "npm não é reconhecido"
**Solução:** Instale Node.js do [nodejs.org](https://nodejs.org/) e reinicie o terminal.

### ❌ "Porta 3000 já está em uso"
**Solução:** Use outra porta:
```bash
npm start -- --port 3001
```

### ❌ Erro ao instalar dependências
**Solução:** Limpe o cache e reinstale:
```bash
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

### ❌ Componentes não aparecem
**Solução:** Verifique se o JavaScript está habilitado no navegador.

---

## 📱 Testes Manuais Recomendados

- [ ] Adicionar uma tarefa
- [ ] Adicionar tags à tarefa
- [ ] Marcar tarefa como completa
- [ ] Deletar tarefa
- [ ] Criar nova lista com filtros
- [ ] Editar nome da lista
- [ ] Gerenciar tags (adicionar, editar, deletar)
- [ ] Filtrar tarefas por tags
- [ ] Filtrar tarefas por status
- [ ] Visualizar em mobile

---

## 🚀 Deploy

### Para GitHub Pages:
```bash
npm run build
# Faça upload dos arquivos da pasta 'dist'
```

### Para Vercel:
```bash
# Conectar repositório no Vercel
# Automático: npm run build é executado
```

### Para Netlify:
```bash
# Build command: npm run build
# Publish directory: dist
```

---

## 📞 Suporte

Se encontrar problemas:

1. Verifique o [README.md](./README.md)
2. Verifique o [VALIDATION_REPORT.md](./VALIDATION_REPORT.md)
3. Abra uma issue no GitHub

---

## ✨ Próximos Passos

- [ ] Testar a aplicação localmente
- [ ] Fazer deploy em produção
- [ ] Configurar backup automático
- [ ] Adicionar mais idiomas (i18n)
- [ ] Implementar sincronização na nuvem

---

**Aproveite o Painel de Tarefas em português! 🇧🇷**
