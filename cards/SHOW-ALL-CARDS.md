# 🎴 Show All Cards - Visualizador Completo

Visualize todas as cartas de rituais de uma só vez em um grid responsivo.

## 🚀 Como Usar

1. **Inicie o json-server** (se não estiver rodando):
```bash
npm run server
```

2. **Abra o arquivo no navegador**:
```
cards/show-all-cards.html
```

3. **Visualize todas as cartas**:
   - Carrega automaticamente todos os rituais
   - Exibe em grid com gap de 0.5rem
   - Layout responsivo

## ✨ Características

### 📊 Layout
- **Grid Responsivo**: Ajusta automaticamente para tela
- **Gap**: 0.5rem entre cards
- **Auto-fill**: Colunas se adaptam ao tamanho da tela
- **Centralizado**: Cards alinhados perfeitamente

### 🎨 Visual
- **Cores por Elemento**: Cada card com cor do elemento
- **Todas as Funcionalidades**: Mesmas features do gerador
  - Fonte dinâmica (descrição e upgrades)
  - Cores por elemento
  - Fallback de imagens
  - Formatação de atributos

### 📱 Responsivo
- **Desktop**: Grid multi-coluna
- **Tablet**: Adapta número de colunas
- **Mobile**: Single column

## 🎯 Casos de Uso

### 📸 Impressão/Exportação
Perfeito para:
- Imprimir múltiplas cartas de uma vez
- Criar PDFs com todas as cartas
- Capturar screenshots do conjunto

### 👀 Revisão
- Ver todos os rituais lado a lado
- Comparar designs e cores
- Verificar consistência visual
- Encontrar erros de formatação

### 🎮 Gameplay
- Ter todas as cartas visíveis durante o jogo
- Buscar rapidamente um ritual específico
- Ver opções disponíveis por elemento

## 🔧 Detalhes Técnicos

### Grid CSS
```css
.cards-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(420px, 1fr));
  gap: 0.5rem;
}
```

### Carregamento
- Faz uma única chamada à API
- Renderiza todos os cards dinamicamente
- Aplica estilos e funções automaticamente

### Performance
- Carrega todas as imagens em paralelo
- Usa fallback para imagens ausentes
- Ajusta fonte dinamicamente em cada card

## 📊 Informações Exibidas

Cada card mostra:
- ✅ Nome do ritual
- ✅ Elemento e círculo
- ✅ Todos os atributos (execução, alcance, alvo, etc)
- ✅ Imagem (quando disponível)
- ✅ Descrição completa
- ✅ Upgrades (Discente e Verdadeira)

## 💡 Dicas

### Para Imprimir
1. Abra `show-all-cards.html`
2. Use `Ctrl/Cmd + P`
3. Configure:
   - Orientação: Retrato ou Paisagem
   - Escala: Ajustar à página
   - Margens: Mínimas

### Para Screenshots
1. Use extensão de captura de página inteira
2. Ou role e capture seções
3. Formato recomendado: PNG ou PDF

### Para Comparação
1. Abra em tela grande
2. Use Ctrl/Cmd + Scroll para zoom
3. Role para ver todos os rituais

## 🆚 Diferenças do Gerador

| Característica | show-all-cards.html | gerador.html |
|----------------|---------------------|--------------|
| Visualização | Todos de uma vez | Um por vez |
| Seleção | Automática | Manual (dropdown) |
| Scroll | Vertical | Não necessário |
| Uso ideal | Revisão/Impressão | Navegação individual |
| Carregamento | Uma vez | Por demanda |

## 🎨 Personalização

### Ajustar Gap
Edite no CSS:
```css
gap: 0.5rem; /* Altere para 1rem, 2rem, etc */
```

### Ajustar Colunas
Edite no CSS:
```css
grid-template-columns: repeat(auto-fill, minmax(420px, 1fr));
                                              /* ↑ altere este valor */
```

### Ordenação
Os rituais aparecem na ordem do `db.json`. Para reordenar:
1. Edite o `db.json`
2. Ou adicione sort no JavaScript

---

**Perfeito para ter uma visão completa de todos os rituais!** 🎴✨

