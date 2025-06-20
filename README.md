# 🛡️ Desafio: Classificador de Nível de Herói

Este desafio foi um projeto desenvolvido como parte de lógica em JavaScript.  
O objetivo é  utilizar:

---

## 🚀 Tecnologias Utilizadas

- ✅ JavaScript
- ✅ Variáveis (`nome/xp/nivel/herois/i`)
- ✅ Operadores lógicos e relacionais (`>=/<=/</&&`)
- ✅ Laço de repetição (`for`)
- ✅ Estruturas de decisão (`if / else if`)
  
---

## 📋 Regras de Classificação

A classificação do herói é feita de acordo com sua quantidade de XP:

| Faixa de XP       | Nível        |
|-------------------|--------------|
| Menor que 1.000   | Ferro        |
| 1.001 a 2.000     | Bronze       |
| 2.001 a 5.000     | Prata        |
| 5.001 a 7.000     | Ouro         |
| 7.001 a 8.000     | Platina      |
| 8.001 a 9.000     | Ascendente   |
| 9.001 a 10.000    | Imortal      |
| 10.001 ou mais    | Radiante     |

---

## 💡 Exemplo de Código

```javascript
let herois = [
    { nome: "William", xp: 6500 },
    { nome: "Sara", xp: 1500 },
    { nome: "Gael", xp: 2500 },
    { nome: "Theo", xp: 10500 }
];

for (let i = 0; i < herois.length; i++) {
    let nome = herois[i].nome;
    let xp = herois[i].xp;
    let nivel = "";

    if (xp < 1000) {
        nivel = "Ferro";
    }
      else if (xp >= 1001 && xp <= 2000) {
        nivel = "Bronze";
    }
      else if (xp >= 2001 && xp <= 5000) {
        nivel = "Prata";
    }
      else if (xp >= 5001 && xp <= 7000) {
        nivel = "Ouro";
    }
      else if (xp >= 7001 && xp <= 8000) {
        nivel = "Platina";
    }
      else if (xp >= 8001 && xp <= 9000) {
        nivel = "Ascendente";
    }
      else if (xp >= 9001 && xp <= 10000) {
        nivel = "Imortal";
    }
      else {
        nivel = "Radiante";
    }

    console.log(`O Herói de nome ${nome} está no nível de ${nivel}`);
}

//O Herói de nome William está no nível de Ouro  
//O Herói de nome Sara está no nível de Bronze  
//O Herói de nome Gael está no nível de Prata  
//O Herói de nome Theo está no nível de Radiante  
