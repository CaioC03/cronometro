# ⏱️ Cronômetro JavaScript

Este é um projeto simples de cronômetro (timer) implementado em JavaScript puro. Ele conta minutos, segundos e milissegundos, e possui botões para iniciar, pausar, retomar e resetar o cronômetro.

## 🚀 Funcionalidades

- Iniciar a contagem do tempo
- Pausar o cronômetro
- Retomar a contagem após a pausa
- Resetar o cronômetro
- Atualização em tempo real de minutos, segundos e milissegundos

## 🧠 Como funciona

O cronômetro usa `setInterval` para incrementar o tempo a cada 10 milissegundos, simulando um comportamento de contagem precisa. Os valores são exibidos dinamicamente na tela com base nos elementos HTML.

## 📁 Estrutura do Código

### Elementos HTML

O script interage com os seguintes elementos identificados por `id`:

- `#minutes`: exibe os minutos
- `#seconds`: exibe os segundos
- `#milliseconds`: exibe os milissegundos
- `#startBtn`: botão para iniciar
- `#pauseBtn`: botão para pausar
- `#resumeBtn`: botão para retomar
- `#resetBtn`: botão para resetar

### Principais Funções

| Função             | Descrição                                      |
|--------------------|-----------------------------------------------|
| `startTimer()`     | Inicia o cronômetro                           |
| `pauseTimer()`     | Pausa a contagem sem resetar os valores       |
| `resumeTimer()`    | Retoma o cronômetro de onde parou             |
| `resetTimer()`     | Para a contagem e zera os valores             |
| `formatTime()`     | Formata números com dois dígitos (ex: 4 → 04) |
| `formatMilliseconds()` | Formata os milissegundos com três dígitos (ex: 5 → 005) |

> ⚠️ A função `formatMilliseconds()` está definida mas não é utilizada no código atual.

## 🛠️ Como usar

1. Crie um arquivo HTML com os elementos correspondentes (`#minutes`, `#seconds`, `#milliseconds`, botões).
2. Vincule o script ao HTML.
3. Abra o arquivo HTML no navegador e utilize os botões para controlar o cronômetro.

## 💡 Exemplo de HTML

```html
<div>
  <span id="minutes">00</span>:<span id="seconds">00</span>:<span id="milliseconds">000</span>
</div>
<button id="startBtn">Iniciar</button>
<button id="pauseBtn" style="display:none;">Pausar</button>
<button id="resumeBtn" style="display:none;">Retomar</button>
<button id="resetBtn">Resetar</button>
