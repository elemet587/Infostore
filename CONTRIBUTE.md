# 🤝 Guia de Contribuição - Infostore

Obrigado pelo interesse em contribuir com o projeto Infostore! Este guia vai te ajudar a começar.

## 📋 Índice

- [Como Contribuir](#como-contribuir)
- [Tipos de Contribuição](#tipos-de-contribuição)
- [Processo de Desenvolvimento](#processo-de-desenvolvimento)
- [Padrões de Código](#padrões-de-código)
- [Reportar Bugs](#reportar-bugs)
- [Sugerir Funcionalidades](#sugerir-funcionalidades)
- [Pull Requests](#pull-requests)
- [Comunidade](#comunidade)

## 🚀 Como Contribuir

### 1. Fork do Repositório

```bash
# Clique em "Fork" no GitHub ou use o GitHub CLI
gh repo fork Emicy963/Infostore --clone
```

### 2. Configurar Ambiente Local

```bash
# Clone seu fork
git clone https://github.com/Emicy963/Infostore.git
cd infostore-landing

# Adicionar repositório original como upstream
git remote add upstream https://github.com/Emicy963/Infostore.git
```

### 3. Criar Branch para Feature

```bash
# Sempre criar branch a partir da main atualizada
git checkout main
git pull upstream main
git checkout -b feature/nome-da-sua-feature
```

## 🎯 Tipos de Contribuição

### 🐛 Correção de Bugs

- Identifique e corrija problemas no código
- Teste a correção em diferentes dispositivos
- Documente a correção no PR

### ✨ Novas Funcionalidades

- Melhorias na UI/UX
- Otimizações de performance
- Novas seções ou componentes
- Integração com APIs

### 📚 Documentação

- Melhorar README.md
- Adicionar comentários no código
- Criar tutoriais ou guias
- Traduzir documentação

### 🎨 Design

- Melhorias visuais
- Responsividade
- Acessibilidade
- Animações e transições

## ⚙️ Processo de Desenvolvimento

### 1. Planejamento

- Abra uma issue para discutir grandes mudanças
- Verifique se não existe issue/PR similar
- Defina escopo e objetivos claros

### 2. Desenvolvimento

```bash
# Mantenha branch atualizada
git pull upstream main
git rebase main

# Faça commits pequenos e descritivos
git add .
git commit -m "feat: adicionar seção de depoimentos"
```

### 3. Testes

- Teste em diferentes navegadores (Chrome, Firefox, Safari)
- Verifique responsividade (mobile, tablet, desktop)
- Valide acessibilidade básica
- Teste performance (PageSpeed Insights)

### 4. Submissão

```bash
# Push da branch
git push origin feature/nome-da-sua-feature

# Abrir Pull Request no GitHub
```

## 📏 Padrões de Código

### HTML

```html
<!-- Use estrutura semântica -->
<section class="py-16">
    <div class="max-w-7xl mx-auto px-4">
        <h2 class="text-3xl font-bold mb-8">Título da Seção</h2>
        <!-- Conteúdo -->
    </div>
</section>
```

### CSS (Tailwind)

```html
<!-- Prefira classes utilitárias do Tailwind -->
<div class="bg-white rounded-lg shadow-md hover:shadow-lg transition-shadow">
    <!-- Use classes responsivas -->
    <h3 class="text-lg md:text-xl lg:text-2xl font-semibold">
        Título Responsivo
    </h3>
</div>
```

### JavaScript

```javascript
// Use JavaScript moderno (ES6+)
const produtos = document.querySelectorAll('.produto-card');

produtos.forEach(produto => {
    produto.addEventListener('click', handleProdutoClick);
});

// Funções descritivas
function handleProdutoClick(event) {
    // Lógica do clique
}
```

### Convenções de Nomenclatura

- **Classes CSS**: `kebab-case` (ex: `produto-card`)
- **IDs**: `camelCase` (ex: `produtoDestaque`)
- **Funções JS**: `camelCase` (ex: `handleFormSubmit`)
- **Constantes**: `UPPER_CASE` (ex: `API_URL`)

## 🐛 Reportar Bugs

### Template de Bug Report

```markdown
**Descrição do Bug**
Descrição clara e concisa do problema.

**Passos para Reproduzir**
1. Vá para '...'
2. Clique em '...'
3. Role até '...'
4. Veja o erro

**Comportamento Esperado**
O que deveria acontecer.

**Screenshots**
Se aplicável, adicione screenshots.

**Ambiente:**
- Dispositivo: [ex: iPhone 12]
- Navegador: [ex: Chrome 95]
- Versão: [ex: 1.2.0]

**Contexto Adicional**
Qualquer outra informação relevante.
```

## 💡 Sugerir Funcionalidades

### Template de Feature Request

```markdown
**A funcionalidade está relacionada a um problema?**
Descrição clara do problema. Ex: "Fico frustrado quando..."

**Descreva a solução desejada**
Descrição clara e concisa do que você quer que aconteça.

**Descreva alternativas consideradas**
Descrição de soluções ou funcionalidades alternativas.

**Contexto Adicional**
Screenshots, mockups, ou contexto adicional.
```

## 🔄 Pull Requests

### Checklist do PR

- [ ] Código segue os padrões estabelecidos
- [ ] Testado em diferentes dispositivos
- [ ] Documentação atualizada (se necessário)
- [ ] Commits são descritivos
- [ ] Não quebra funcionalidades existentes
- [ ] Performance não foi afetada negativamente

### Template de PR

```markdown
## Descrição
Breve descrição das mudanças realizadas.

## Tipo de Mudança
- [ ] Bug fix
- [ ] Nova funcionalidade
- [ ] Mudança que quebra compatibilidade
- [ ] Documentação

## Como Testar
1. Passos para testar as mudanças
2. Cenários específicos
3. Dispositivos/navegadores testados

## Screenshots
Se aplicável, adicione screenshots das mudanças.

## Checklist
- [ ] Código segue padrões do projeto
- [ ] Testado localmente
- [ ] Documentação atualizada
```

## 📱 Prioridades Atuais

### Alta Prioridade

- 🔧 Otimização de performance
- 📱 Melhorias de responsividade
- ♿ Acessibilidade (WCAG 2.1)
- 🌐 Suporte para PWA

### Média Prioridade

- 🎨 Animações e micro-interações
- 📊 Analytics e métricas
- 🔍 SEO improvements
- 🌍 Internacionalização (i18n)

### Baixa Prioridade

- 🎮 Easter eggs
- 🎨 Temas alternativos
- 📈 Dashboards avançados

## 🌟 Reconhecimento

Contribuidores serão reconhecidos:

- 📜 Lista de contribuidores no README
- 🏆 Badges especiais no perfil GitHub
- 📢 Menção nas release notes
- 🎁 Brindes da Infostore (para contribuições significativas)

## 🤔 Precisa de Ajuda?

### Canais de Comunicação

- 📧 **Email**: [andersonpaulo931@gmail.com](andersonpaulo931@gmail.com)
- 💬 **Linkedin**: [Anderson Cafurica](https://https://github.com/Emicy963/)
- 📱 **WhatsApp**: [+244 928 301 450](https://wa.me/244928301450)

### Recursos Úteis

- [Tailwind CSS Docs](https://tailwindcss.com/docs)
- [MDN Web Docs](https://developer.mozilla.org/)
- [GitHub Docs](https://docs.github.com/)
- [Conventional Commits](https://www.conventionalcommits.org/)

## 🎯 Metas da Comunidade

### 2025 Q1

- [ ] 10+ contribuidores ativos
- [ ] 50+ estrelas no GitHub
- [ ] 100% cobertura de responsividade
- [ ] Score 95+ no Lighthouse

### 2025 Q2

- [ ] Migração para e-commerce
- [ ] API backend integrada
- [ ] Sistema de pagamentos
- [ ] App mobile MVP

---

**Juntos construímos uma melhor experiência tecnológica para Angola! 🇦🇴✨**

Obrigado por contribuir com o projeto Infostore! 🙏