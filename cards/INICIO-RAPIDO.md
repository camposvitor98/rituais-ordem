# 🎴 Início Rápido - Gerador de Cartas

## Passo a Passo

### 1️⃣ O json-server já está rodando!
✅ Servidor ativo em `http://localhost:3000`

### 2️⃣ Abrir o visualizador

**Opção A - Seleção Individual:**
```
/Users/campos.vitor98/github/Ordem paranormal/Script/cards/gerador.html
```

**Opção B - Ver Todas as Cartas:**
```
/Users/campos.vitor98/github/Ordem paranormal/Script/cards/show-all-cards.html
```

Ou clique com botão direito em qualquer arquivo → "Abrir com..." → Navegador

### 3️⃣ Usar o sistema

**Gerador (gerador.html):**
1. Selecione um ritual no dropdown
2. O card será gerado automaticamente
3. Todas as informações virão do `db.json`

**Visualizar Tudo (show-all-cards.html):**
1. Todos os rituais aparecem em grid
2. Gap de 0.5rem entre cards
3. Layout responsivo automático

## 🎯 O que foi criado

### `gerador.html`
- **Interface interativa** com dropdown de seleção
- **Renderização dinâmica** dos cards
- **Integração com json-server** (API REST)
- **Design responsivo** igual ao card.html original
- **Cores automáticas** por elemento (Sangue, Morte, Conhecimento, etc)

## 🎨 Funcionalidades

✨ **Seleção Inteligente**
- Dropdown organizado alfabeticamente
- Mostra elemento e círculo de cada ritual
- Remove duplicatas automaticamente

✨ **Renderização Automática**
- Título, elemento e círculo
- Todos os atributos (execução, alcance, alvo, etc)
- Descrição completa
- Upgrades (Discente e Verdadeira)
- Imagens (quando disponíveis)

✨ **Cores por Elemento**
- 🟡 Conhecimento (amarelo)
- 🟣 Energia (roxo)
- ⚫ Morte (preto)
- 🔴 Sangue (vermelho)
- ⚪ Medo (branco)

## 📸 Exemplo de Uso

```
1. Abrir gerador.html
2. Selecionar "Corpo Adaptado (Sangue • Círculo 1)"
3. Card vermelho aparece com todos os dados
4. Selecionar outro ritual
5. Card muda automaticamente
```

## 🔧 Comandos Úteis

```bash
# Iniciar servidor (se não estiver rodando)
npm run server

# Parar servidor
Ctrl + C no terminal

# Editar rituais
# Edite db.json e o gerador atualizará automaticamente
```

## 💡 Dicas

- Os rituais são carregados diretamente do `db.json`
- Para adicionar/editar rituais, edite o `db.json`
- As imagens devem estar em `cards/assets/`
- Nome da imagem: **ID do ritual** + `.webp` (ex: `corpo-adaptado.webp`, `compreensao-paranormal.webp`)
- O ID já está normalizado no `db.json` (lowercase, sem acentos, com hífens)

---

**Pronto para usar! 🚀**

