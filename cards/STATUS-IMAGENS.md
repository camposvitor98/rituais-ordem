# 📸 Status das Imagens dos Rituais

## ✅ Imagens Configuradas

Total de rituais: **27**
Imagens presentes: **26** (96%)
Imagens faltando: **1** (4%)

## ❌ Imagem Faltando

### Convocar o Algoz
- **ID**: `convocar-o-algoz`
- **Arquivo necessário**: `assets/convocar-o-algoz.webp`
- **Status**: Quando selecionado, mostrará "Sem imagem"

## ✅ Rituais com Múltiplos Elementos

Os seguintes rituais têm variantes para diferentes elementos e suas imagens foram duplicadas:

### Amaldiçoar Arma
- `amaldicoar-arma.webp` (Conhecimento - original)
- `amaldicoar-arma-energia.webp` ✅
- `amaldicoar-arma-morte.webp` ✅
- `amaldicoar-arma-sangue.webp` ✅

## 🔧 Como Adicionar a Imagem Faltando

1. Crie ou obtenha a imagem do ritual "Convocar o Algoz"
2. Converta para formato `.webp`
3. Renomeie para `convocar-o-algoz.webp`
4. Coloque em `cards/assets/`
5. Recarregue o gerador

## 🧪 Teste de Imagens

Um arquivo de teste foi criado para verificar o carregamento de todas as imagens:

```
cards/teste-imagens.html
```

Abra este arquivo no navegador com o json-server rodando para ver o status de cada imagem.

## 📋 Lista Completa de Imagens

Todas as imagens seguem o padrão: `{id-do-ritual}.webp`

```
✅ alterar-destino.webp
✅ alterar-memoria.webp
✅ amaldicoar-arma.webp
✅ amaldicoar-arma-energia.webp (duplicada)
✅ amaldicoar-arma-morte.webp (duplicada)
✅ amaldicoar-arma-sangue.webp (duplicada)
✅ amaldicoar-tecnologia.webp
✅ ancora-temporal.webp
✅ aprimorar-fisico.webp
✅ aprimorar-mente.webp
✅ arma-atroz.webp
✅ armadura-de-sangue.webp
✅ canalizar-o-medo.webp
✅ capturar-o-coracao.webp
✅ chamas-do-caos.webp
✅ cicatrizacao.webp
✅ cineraria.webp
✅ coincidencia-forcada.webp
✅ compreensao-paranormal.webp
✅ conhecendo-o-medo.webp
✅ consumir-manancial.webp
✅ contato-paranormal.webp
✅ contencao-fantasmagorica.webp
✅ controle-mental.webp
✅ convocacao-instantanea.webp
❌ convocar-o-algoz.webp (FALTANDO)
✅ corpo-adaptado.webp
```

## 💡 Notas

- O sistema já está preparado para lidar com imagens faltando
- Mostra "Sem imagem" como fallback
- As imagens são carregadas automaticamente quando disponíveis
- Não é necessário reiniciar o servidor ao adicionar novas imagens

