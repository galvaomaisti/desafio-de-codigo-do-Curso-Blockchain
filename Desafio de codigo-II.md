# Desafio A Companhia de Táxi Tabajara (CTT) é:

- **Entrada  é composta por uma linha contendo quatro números reais com precisão de duas casas decimais A e G (0.01 ≤ A, G ≤ 10.00) Ra e Rg (0.01 ≤ Ra , Rg ≤ 20.00) representando respectivamente o preço por litro do álcool, o preço por litro da gasolina, o rendimento (km/l) do carro utilizando álcool e o rendimento (km/l) do carro utilizando gasolina.)**

- **Saída
A saída deve ser composta por uma única linha contendo o caractere ‘A’ se é mais econômico abastecer a frota com álcool ou o caractere ‘G’ se é mais econômico ou indiferente abastecer a frota com gasolina.

A saída deve ser escrita no dispositivo de saída padrão (normalmente a tela).

 
Exemplos de Entrada	Exemplos de Saída
1.20 2.30 10.00 15.00	A
1.00 1.00 9.00 9.01	G
1.00 1.00 11.00 11.00	G
 
OBI - Olimpíada Brasileira de Informática 2005 Nível 1

**

- **Solução do Codigo
// IMPORTANTE: As funções "gets" e "print" são acessíveis globalmente e têm as seguintes funcionalidades: 
// - "gets" : lê UMA linha com dados de entrada (inputs) do usuário;
// - "print": imprime um texto de saída (output) e pula uma linha ("\n") automaticamente;
// Abaixo segue o template de código para este desafio, o qual pode ou não utilizar tais funções.

//let linha = gets();

// Atribui os valores de entrada nas respectivas constantes usando destructuring.
// Referencia: https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment
//const [precoAlcool, precoGasolina, rendimentoAlcool, rendimentoGasolina] = 
  //linha.split(' ').map(x => parseFloat(x));

//TODO: Calcular o Preço/Km para cada conbustível considerando os valores de entrada.
//const precoPorKmAlcool = 0;
//const precoPorKmGasolina = 0;

// Usa o conceito de operador condicional (ternário) para identificar qual é o melhor preço.
// Referência: https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Conditional_Operator
//const maisEconomico = precoPorKmGasolina <= precoPorKmAlcool ? 'G' : 'A';
//print(maisEconomico);

let lines = gets().split('\n');
const [precoAlcool, precoGasolina, rendimentoAlcool, rendimentoGasolina] = lines[0].split(' ').map(x => parseFloat(x));
const precoPorKmAlcool =  precoAlcool / rendimentoAlcool;
const precoPorKmGasolina = precoGasolina /  rendimentoGasolina;
const maisEconomico = precoPorKmGasolina <= precoPorKmAlcool ? 'G' : 'A';
print(maisEconomico);**

- **Desafio de projeto( =>)**

  