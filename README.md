# 🕹️ Calculadora de Partidas Rankeadas

Projeto desenvolvido como parte do bootcamp da **DIO (Digital Innovation One)**.  
O objetivo deste projeto é criar um sistema que calcula o saldo de partidas rankeadas de um jogador e classifica seu nível de acordo com a quantidade de vitórias.

---

## 🎯 Objetivo

- Criar uma função que recebe como parâmetros a quantidade de **vitórias** e **derrotas** de um jogador.
- Calcular o **saldo de vitórias**:  
saldo = vitórias - derrotas

bash
Copiar código
- Classificar o jogador em um **nível** baseado no número de vitórias.

---

## 🧩 Regras de Classificação

| Vitórias | Nível       |
|----------|------------|
| < 10     | Ferro      |
| 11–20    | Bronze     |
| 21–50    | Prata      |
| 51–80    | Ouro       |
| 81–90    | Diamante   |
| 91–100   | Lendário   |
| ≥101     | Imortal    |

---

## 💻 Código Fonte (JavaScript)

```javascript
function calcularNivel(vitorias, derrotas) {
  let saldoVitorias = vitorias - derrotas;
  let nivel = "";

  if (vitorias < 10) {
      nivel = "Ferro";
  } else if (vitorias <= 20) {
      nivel = "Bronze";
  } else if (vitorias <= 50) {
      nivel = "Prata";
  } else if (vitorias <= 80) {
      nivel = "Ouro";
  } else if (vitorias <= 90) {
      nivel = "Diamante";
  } else if (vitorias <= 100) {
      nivel = "Lendário";
  } else {
      nivel = "Imortal";
  }

  return `O Herói tem de saldo de ${saldoVitorias} está no nível de ${nivel}`;
}

// Exemplo de uso
let vitorias = 55;
let derrotas = 20;
console.log(calcularNivel(vitorias, derrotas));
📤 Exemplo de Saída
nginx
Copiar código
O Herói tem de saldo de 35 está no nível de Ouro
🚀 Tecnologias Utilizadas
JavaScript

Node.js (opcional para execução local)

📚 Aprendizados
Uso de funções para modularizar a lógica

Estruturas de decisão (if / else if / else)

Manipulação de variáveis e operadores

Retorno de valores a partir de funções

Formatação de saída para exibição de resultados

👨‍💻 Autor
Projeto desenvolvido por Mykoll
Bootcamp DIO