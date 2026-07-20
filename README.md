# Painel de Tarefas

Uma aplicação de gerenciamento de tarefas que permite aos usuários criar, organizar e filtrar tarefas usando uma interface moderna e responsiva construída com React.

> **Nota:** Esta aplicação é destinada apenas para fins de demonstração e não se destina ao uso em produção.

## Recursos

- **Gerenciamento de Tarefas**: Criar, completar e deletar tarefas
- **Tags de Tarefas**: Organizar tarefas com tags personalizáveis
- **Listas de Tarefas**: Criar múltiplas listas com filtros personalizados
- **Filtros de Lista**: Filtrar tarefas por tags ou status de conclusão
- **Animações**: Transições suaves e animações usando Framer Motion
- **Design Responsivo**: Funciona em dispositivos desktop e mobile

## Pilha Tecnológica

- **React**: React moderno com componentes funcionais e hooks
- **Tailwind CSS**: Framework CSS first-utility para estilização
- **Framer Motion**: Biblioteca de animação para React
- **Vite**: Ferramenta de build rápida e moderna e servidor de desenvolvimento
- **Vitest**: Framework de teste compatível com Vite

## Começando

### Pré-requisitos

- Node.js (v18+)
- npm (v10+)

### Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/painel-tarefas.git
   cd painel-tarefas
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Inicie o servidor de desenvolvimento:
   ```bash
   npm start
   ```

4. Abra [http://localhost:3000](http://localhost:3000) para visualizar o aplicativo

### Scripts Disponíveis

- `npm start` - Inicie o servidor de desenvolvimento
- `npm start:hydrated` - Inicie o servidor de desenvolvimento com hidratação de dados ativada
- `npm run build` - Crie para produção
- `npm run build:hydrated` - Crie para produção com hidratação de dados ativada
- `npm run build:clean` - Crie para produção com hidratação de dados explicitamente desativada
- `npm run preview` - Visualize o build de produção localmente
- `npm run preview:hydrated` - Visualize o build de produção com hidratação de dados ativada
- `npm test` - Execute testes com Vitest

### Hidratação de Dados

A aplicação oferece suporte a pré-preenchimento com dados de amostra através de um processo de hidratação opcional:

- Os dados de amostra são definidos em `src/data/initialData.json`
- A hidratação pode ser ativada/desativada usando a variável de ambiente `VITE_ENABLE_DATA_HYDRATION`
- Use os scripts de conveniência para desenvolvimento com hidratação:
  - `npm run start:hydrated` - Desenvolvimento com dados de amostra
  - `npm run build:hydrated` - Build de produção com dados de amostra
  - `npm run build:clean` - Build de produção sem dados de amostra
- A implantação do GitHub Actions ativa automaticamente a hidratação para o build de produção

## Arquitetura

### Gerenciamento de Estado

A aplicação usa React Context para gerenciamento de estado:

- **TaskContext**: Gerencia o estado de tarefas e operações (adicionar, alternar, deletar)
- **TagContext**: Gerencia tags e suas relações com tarefas
- **ListContext**: Gerencia listas de tarefas e lógica de filtragem

### Componentes da Interface

A aplicação apresenta vários componentes-chave:
- **TaskList**: Renderiza uma lista de tarefas
- **TaskItem**: Renderiza uma tarefa individual
- **TaskBoard**: Gerencia múltiplas listas de tarefas
- **TagManager**: Interface para criar e gerenciar tags
- **GlobalTaskForm**: Formulário para criar novas tarefas
- **ListAddTask**: Formulário para adicionar tarefas a listas específicas
- **TaskListConfig**: Interface para configurar listas de tarefas

## Contribuindo

1. Faça fork do repositório
2. Crie seu branch de feature (`git checkout -b feature/recurso-incrivel`)
3. Faça commit das suas mudanças (`git commit -m 'Adicione algum recurso incrível'`)
4. Faça push para o branch (`git push origin feature/recurso-incrivel`)
5. Abra um Pull Request

## Licença

Este projeto é licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.
