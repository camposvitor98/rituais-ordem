# Gerador de Cartas de Rituais - Ordem Paranormal

Sistema para visualizar cartas de rituais do RPG Ordem Paranormal com dados dinâmicos do json-server.

## 🚀 Como Usar

### 1. Iniciar o JSON Server

No terminal, execute:

```bash
npm run server
```

O servidor iniciará em `http://localhost:3000`

### 2. Abrir o Gerador

Abra o arquivo `gerador.html` no seu navegador:

```
cards/gerador.html
```

**Ou** para ver todas as cartas de uma vez:

```
cards/show-all-cards.html
```

### 3. Selecionar um Ritual (gerador.html)

- Use o dropdown para selecionar um ritual
- O card será renderizado automaticamente com:
  - **Título** e **elemento** colorido
  - **Atributos** (execução, alcance, alvo, duração, resistência)
  - **Imagem** do ritual (se existir em `assets/`)
  - **Descrição** completa
  - **Upgrades** (Discente e Verdadeira)

## 🎨 Elementos e Cores

Cada elemento possui uma cor específica:

- **Conhecimento**: Amarelo (`#eab308`)
- **Energia**: Roxo (`#7c3aed`)
- **Morte**: Preto (`#18181b`)
- **Sangue**: Vermelho (`#dc2626`)
- **Medo**: Branco (`#f5f5f5` com sombra para contraste)

## 📁 Estrutura

```
cards/
├── gerador.html          # Gerador interativo (seleção individual)
├── show-all-cards.html   # Visualizar todas as cartas em grid (NOVO)
├── card.html             # Exemplo estático
├── assets/               # Imagens dos rituais
│   ├── corpo-adaptado.webp
│   ├── alterar-destino.webp
│   └── ...
```

## 🔧 Requisitos

- **json-server** rodando na porta 3000
- Arquivo `db.json` com os dados dos rituais
- Imagens dos rituais em `cards/assets/` (opcional)

## 📝 Formato das Imagens

As imagens devem seguir o padrão:
- Nome do arquivo: **ID do ritual** (já normalizado no db.json)
- Formato: `.webp`
- Exemplo: 
  - Ritual: "Corpo Adaptado" (ID: `corpo-adaptado`)
  - Imagem: `corpo-adaptado.webp`
  - Ritual: "Compreensão Paranormal" (ID: `compreensao-paranormal`)
  - Imagem: `compreensao-paranormal.webp`

## ✨ Funcionalidades

- ✅ Seleção dinâmica de rituais via API
- ✅ Renderização automática com cores por elemento
- ✅ Formatação correta de atributos
- ✅ Extração automática de custos de PE
- ✅ Fallback para imagens ausentes
- ✅ Design responsivo
- ✅ Agrupamento de rituais duplicados
- ✅ **Ajuste automático de fonte** (10px a 14px baseado no comprimento)
  - Descrição principal
  - Upgrades (Discente e Verdadeira)

## 🐛 Solução de Problemas

### "Erro ao carregar rituais"
- Verifique se o json-server está rodando: `npm run server`
- Confirme que está acessando `http://localhost:3000`

### Imagem não aparece
- Verifique se o arquivo existe em `cards/assets/`
- Confirme se o nome do arquivo está correto (lowercase, sem acentos)
- O sistema mostrará "Sem imagem" como fallback

## 🎯 Próximos Passos

Possíveis melhorias:
- [ ] Exportar card como imagem PNG
- [ ] Filtros por elemento/círculo
- [ ] Modo de impressão otimizado
- [ ] Editor de rituais inline
- [ ] Geração de baralho completo

