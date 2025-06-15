# Festejando a Conexão Campo-Cidade 🌾🏙️

## 📋 Sobre o Projeto

Este projeto foi desenvolvido para o **Concurso Agrinho 2025**, celebrando a interdependência entre o campo e a cidade através de um site estático responsivo e visualmente atraente. O site explora como a agricultura urbana e rural se conectam, destacando a importância dessa relação para nossa sociedade.

## 🔗 Acesso ao Projeto
https://hyagox.github.io/agrinho-2025-campo-cidade/

### 🎯 Objetivo

Criar uma experiência digital que demonstre como campo e cidade são complementares, explorando:
- A importância da agricultura para o abastecimento urbano
- A troca cultural e econômica entre os dois espaços
- Soluções sustentáveis que conectam ambos os ambientes
- A celebração dessa conexão vital para nossa sociedade

## 🌐 Como Navegar no Site

### Estrutura do Site

1. **Início (Hero)** - Apresentação principal com título criativo e visual impactante
2. **Conexão** - Explora a dança entre campo e cidade através de cards informativos
3. **Agricultura** - Destaca a importância da agricultura com estatísticas e ilustrações
4. **Sustentabilidade** - Apresenta soluções como feiras orgânicas, turismo rural e hortas urbanas
5. **Contato** - Formulário de contato simulado para engajamento

### Navegação Responsiva

- **Desktop**: Menu horizontal fixo no topo
- **Mobile/Tablet**: Menu hamburguer (CSS-only) com animações suaves
- **Acessibilidade**: Navegação por teclado e foco visível

## 🎨 Design e Estilo Visual

### Paleta de Cores

- **Campo**: Tons de verde (#2d5016, #4a7c21, #7ba05b)
- **Cidade**: Tons de azul (#1a365d, #2b77ad, #63b3ed)
- **Neutros**: Branco, cinzas e preto para equilíbrio
- **Destaques**: Dourado (#d69e2e) e terra (#c53030) para acentos

### Tipografia

- **Fonte Principal**: Inter (moderna e legível)
- **Fonte de Destaque**: Playfair Display (elegante para títulos)
- **Hierarquia**: Tamanhos responsivos usando clamp()

### Elementos Visuais

- **Ícones**: Emojis temáticos (🌾, 🏙️, 🤝, 🥕, etc.)
- **Ilustrações**: Elementos gráficos criados com CSS puro
- **Animações**: Transições suaves e efeitos hover
- **Layout**: Grid e Flexbox para organização moderna

## 💻 Técnicas CSS Utilizadas

### Técnicas Avançadas

#### 1. **Variáveis CSS (:root)**
```css
:root {
  --cor-campo: #2d5016;
  --cor-cidade: #1a365d;
  --espacamento-md: 1rem;
  --transicao-media: 0.3s ease-in-out;
}
```

#### 2. **Pseudo-elementos Decorativos**
```css
.section-title::after {
  content: '';
  position: absolute;
  bottom: -0.5rem;
  left: 0;
  width: 4rem;
  height: 3px;
  background: linear-gradient(90deg, var(--cor-campo), var(--cor-cidade));
}
```

#### 3. **Animações com @keyframes**
```css
@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 0.8; }
  50% { transform: scale(1.05); opacity: 1; }
}

@keyframes move-tractor {
  0% { left: -60px; }
  100% { left: calc(100% + 60px); }
}
```

#### 4. **Seletores CSS Avançados**
```css
/* Seletor de atributo */
a[href^="http"]:not([href*="campocidade.com.br"])::after {
  content: " ↗";
}

/* Pseudo-classes estruturais */
.conexao-card:nth-child(odd) {
  animation-delay: 0.1s;
}

.sustentabilidade-card:nth-child(3n+1) {
  border-left: 4px solid var(--cor-campo);
}
```

#### 5. **Grid e Flexbox Responsivos**
```css
.conexao-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: var(--espacamento-xl);
}

.hero-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: var(--espacamento-3xl);
  align-items: center;
}
```

### Responsividade

- **Mobile-first**: Design otimizado para dispositivos móveis
- **Breakpoints**: 320px, 480px, 768px, 1024px
- **Menu Hamburguer**: Implementado apenas com CSS
- **Imagens Responsivas**: Usando técnicas modernas de CSS

### Interatividade (CSS-only)

- **Botões**: Efeitos :hover e :active com transformações
- **Cards**: Elevação e destaque ao passar o mouse
- **Transições**: Animações suaves em todos os elementos interativos
- **Menu Mobile**: Hamburguer animado sem JavaScript

## 🏗️ Estrutura de Arquivos

```
/
├── index.html          # Página principal com HTML semântico
├── style.css           # Estilos CSS completos e responsivos
├── README.md           # Documentação do projeto
```

### HTML Semântico

O código utiliza tags semânticas apropriadas:
- `<header>` e `<nav>` para navegação
- `<main>` para conteúdo principal
- `<section>` para seções temáticas
- `<article>` para conteúdo independente
- `<footer>` para rodapé

## 🌟 Destaques do Projeto

### Originalidade

- **Conceito Visual**: Elementos gráficos únicos criados com CSS
- **Ilustrações Customizadas**: Animação do trator, campos de cultivo
- **Paleta Harmoniosa**: Cores que representam a conexão campo-cidade
- **Micro-interações**: Detalhes que enriquecem a experiência

### Complexidade Técnica

- **Pseudo-elementos**: Decorações e ícones criados com CSS
- **Animações Complexas**: Múltiplas animações sincronizadas
- **Seletores Avançados**: nth-child, attribute selectors, combinadores
- **Responsividade Completa**: Layout fluido em todos os dispositivos

### Acessibilidade

- **Navegação por Teclado**: Foco visível e ordem lógica
- **Contraste**: Cores que atendem padrões de acessibilidade
- **Semântica**: HTML estruturado para leitores de tela
- **Preferências do Usuário**: Respeita `prefers-reduced-motion`

## 🎯 Critérios de Avaliação Atendidos

### Conteúdo (25 pontos)
- ✅ Tema abordado de forma original e criativa
- ✅ Textos autorais sobre conexão campo-cidade
- ✅ Informações relevantes e bem estruturadas
- ✅ Slogan criativo: "Onde a natureza encontra o progresso"

### Design (25 pontos)
- ✅ Layout visualmente atraente e harmônico
- ✅ Paleta de cores coerente com o tema
- ✅ Tipografia legível e hierarquizada
- ✅ Elementos visuais complementam o conteúdo

### Responsividade (20 pontos)
- ✅ Funciona perfeitamente em mobile, tablet e desktop
- ✅ Menu hamburguer para dispositivos móveis
- ✅ Layout adaptativo com Grid e Flexbox
- ✅ Imagens e elementos proporcionais

### Código (20 pontos)
- ✅ HTML semântico e bem estruturado
- ✅ CSS organizado com comentários explicativos
- ✅ Técnicas avançadas implementadas
- ✅ Código limpo e otimizado

### Inovação (10 pontos)
- ✅ Animações criativas com CSS puro
- ✅ Seletores CSS avançados
- ✅ Elementos visuais únicos
- ✅ Micro-interações bem executadas

## 🚀 Como Executar o Projeto

1. **Clone ou baixe os arquivos**
2. **Abra o `index.html` em qualquer navegador moderno**
3. **Ou utilize um servidor local para melhor experiência**

### Servidor Local (Opcional)

```bash
# Com Python 3
python -m http.server 8000

# Com Node.js (npx)
npx serve .

# Com PHP
php -S localhost:8000
```

## 📱 Compatibilidade

### Navegadores Suportados
- ✅ Chrome (versão 90+)
- ✅ Firefox (versão 88+)
- ✅ Safari (versão 14+)
- ✅ Edge (versão 90+)

### Dispositivos Testados
- ✅ Desktop (1200px+)
- ✅ Laptop (1024px - 1199px)
- ✅ Tablet (768px - 1023px)
- ✅ Mobile (320px - 767px)

## 🎨 Créditos e Recursos

### Fontes Utilizadas
- **Inter**: Google Fonts - Fonte principal moderna e legível
- **Playfair Display**: Google Fonts - Fonte elegante para títulos

### Elementos Visuais
- **Ícones**: Emojis Unicode para representação temática
- **Ilustrações**: Elementos gráficos criados inteiramente com CSS
- **Cores**: Paleta desenvolvida especificamente para o projeto
- **Animações**: Todas as animações foram criadas com CSS puro

### Inspirações de Design
- **Agricultura Moderna**: Referências visuais de fazendas sustentáveis
- **Design Urbano**: Elementos que remetem à vida nas cidades
- **Conexão Natural**: Gradientes e transições que simbolizam união

## 🏆 Diferenciais Competitivos

### Técnicos
1. **CSS Puro**: Nenhum JavaScript utilizado, apenas HTML e CSS
2. **Performance**: Otimizado para carregamento rápido
3. **Manutenibilidade**: Código bem documentado e organizado
4. **Escalabilidade**: Estrutura preparada para futuras expansões

### Visuais
1. **Identidade Única**: Design original que representa o tema
2. **Experiência Fluida**: Navegação intuitiva e agradável
3. **Detalhes Cuidadosos**: Micro-interações que encantam
4. **Consistência**: Padrões visuais mantidos em todo o site

### Conceituais
1. **Mensagem Clara**: Comunicação efetiva sobre campo-cidade
2. **Engajamento**: Conteúdo que convida à reflexão
3. **Educativo**: Informações que agregam conhecimento
4. **Inspirador**: Motiva ações sustentáveis

## 📞 Contato

Este projeto foi desenvolvido para o **Concurso Agrinho 2025**, celebrando a importante conexão entre campo e cidade que sustenta nossa sociedade.

**Tags**: #agrinho #campocidade #sustentabilidade #agricultura #responsivo #css #html

---

*Projeto desenvolvido com 💚 para o Concurso Agrinho 2025*
*"Onde a natureza encontra o progresso"*
