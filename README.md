# 🎨 Extractor de Estilo com Gemini

Uma extensão moderna para navegadores que extrai automaticamente os estilos visuais de qualquer página web e gera prompts detalhados usando a API do Google Gemini.

## ✨ Funcionalidades

### 🔍 Extração Inteligente
- **Análise automática** de estilos CSS de qualquer página
- **Extração otimizada** com cache e performance melhorada
- **Suporte completo** a variáveis CSS, cores, tipografia e layout
- **Detecção inteligente** de componentes e padrões de design

### 🤖 Integração com IA
- **Google Gemini 1.5 Flash** para geração de prompts
- **Prompts estruturados** em português com seções organizadas
- **Análise detalhada** de identidade visual, tipografia e componentes
- **Inferências inteligentes** baseadas nos dados extraídos

### 🎯 Interface Moderna
- **Design system completo** com suporte a tema escuro/claro
- **Animações suaves** e micro-interações elegantes
- **Tooltips informativos** com atalhos de teclado
- **Notificações toast** para feedback imediato
- **Loading states** com barras de progresso

### 📤 Exportação Avançada
- **Múltiplos formatos**: TXT, Markdown, JSON
- **Metadados completos** incluindo URL e timestamp
- **Dados estruturados** para reutilização

### 📚 Histórico e Gerenciamento
- **Histórico automático** dos últimos 50 prompts
- **Interface de navegação** com preview e ações
- **Carregamento rápido** de prompts anteriores
- **Exportação individual** de itens do histórico

### ♿ Acessibilidade Completa
- **Navegação por teclado** com atalhos personalizados
- **ARIA labels** e roles para leitores de tela
- **Suporte a `prefers-reduced-motion`**
- **Contraste otimizado** para melhor legibilidade

## 🚀 Instalação

### Pré-requisitos
- Navegador baseado em Chromium (Chrome, Edge, Brave, etc.)
- API Key do Google Gemini ([obter aqui](https://makersuite.google.com/app/apikey))

### Passos de Instalação

1. **Clone ou baixe** este repositório
2. **Abra o navegador** e vá para `chrome://extensions/`
3. **Ative o modo desenvolvedor** no canto superior direito
4. **Clique em "Carregar sem compactação"**
5. **Selecione a pasta** da extensão
6. **Configure sua API key** na primeira utilização

## 🔧 Configuração

### API Key do Gemini
1. Acesse [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Crie uma nova API key
3. Cole a chave na extensão (será salva localmente)
4. Teste a conexão usando o botão "Testar"

### Configurações Avançadas
- **Máximo de elementos**: 50-500 (padrão: 200)
- **Cache**: 0-300 segundos (padrão: 30s)
- **Idioma do prompt**: Português, English, Español
- **Análises opcionais**: Animações, fontes, variáveis CSS
- **Modo debug**: Logs detalhados no console

## 🎮 Como Usar

### Atalhos de Teclado
- `Ctrl + Enter`: Gerar prompt
- `Alt + C`: Copiar resultado
- `Alt + S`: Salvar API key
- `Alt + T`: Alternar visibilidade da chave
- `Escape`: Limpar foco

### Fluxo de Trabalho
1. **Navegue** para qualquer site público
2. **Clique** no ícone da extensão
3. **Pressione** "Gerar prompt com Gemini" ou `Ctrl+Enter`
4. **Aguarde** a análise (com barra de progresso)
5. **Copie** ou **exporte** o resultado

## 📁 Estrutura do Projeto

```
extensão/
├── manifest.json          # Configuração da extensão
├── popup.html            # Interface principal
├── popup.js              # Lógica do popup
├── options.html          # Página de configurações
├── options.js            # Lógica das configurações
├── content_script.js     # Script de extração de estilos
├── INSTRUCOES_INSTALACAO.md  # Guia de instalação
└── README.md             # Este arquivo
```

## 🛠️ Tecnologias Utilizadas

- **Manifest V3** - Última versão da API de extensões
- **Vanilla JavaScript** - Sem dependências externas
- **CSS Custom Properties** - Sistema de design moderno
- **Chrome Extensions API** - Storage, tabs, scripting
- **Google Gemini API** - Geração de prompts com IA

## 🎨 Design System

### Cores
- **Primária**: `#6366f1` (Indigo)
- **Sucesso**: `#10b981` (Emerald)
- **Erro**: `#ef4444` (Red)
- **Texto**: `#1e293b` / `#f8fafc` (Slate)

### Tipografia
- **Família**: System UI stack
- **Tamanhos**: 12px - 32px
- **Pesos**: 400, 500, 600, 700

### Espaçamentos
- **Grid**: 4px base unit
- **Componentes**: 8px, 12px, 16px, 20px, 24px
- **Layout**: 40px, 48px

## 🔒 Privacidade e Segurança

- **Dados locais**: API key armazenada apenas no navegador
- **Sem telemetria**: Nenhum dado enviado para servidores externos
- **HTTPS obrigatório**: Comunicação segura com APIs
- **Permissões mínimas**: Apenas o necessário para funcionamento

## 🐛 Solução de Problemas

### Erro de Conexão
- Recarregue a página e tente novamente
- Verifique se a página permite extensões
- Evite páginas internas do navegador (`chrome://`, `edge://`)

### API Key Inválida
- Verifique o formato: deve começar com "AIza" e ter 39 caracteres
- Teste a chave usando o botão "Testar" nas configurações
- Gere uma nova chave se necessário

### Performance
- Reduza o número máximo de elementos nas configurações
- Desative análises opcionais se não precisar
- Limpe o histórico periodicamente

## 📈 Roadmap

- [ ] Suporte a Firefox (Manifest V2)
- [ ] Análise de responsividade
- [ ] Exportação para Figma/Sketch
- [ ] Templates de prompt personalizáveis
- [ ] Comparação entre páginas
- [ ] Integração com outras IAs

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👨‍💻 Autor

**aajunior43**
- GitHub: [@aajunior43](https://github.com/aajunior43)

## 🙏 Agradecimentos

- Google Gemini pela API de IA
- Comunidade de desenvolvedores de extensões
- Usuários que testaram e forneceram feedback

---

**⭐ Se este projeto foi útil, considere dar uma estrela no GitHub!**