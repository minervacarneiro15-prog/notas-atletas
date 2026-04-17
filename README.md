# notas-atletas
function calcularMedia(notas) {
  let soma = 0;
  for (let nota of notas) {
    soma += nota;
  }
  return soma / notas.length;
}

function main() {
  const nome = prompt("Digite o nome do atleta:");
  const notas = [];

  
  for (let i = 1; i <= 3; i++) {
    const nota = parseFloat(prompt(`Digite a nota ${i}:`));
    notas.push(nota);
  }

  const media = calcularMedia(notas);

  console.log("--- Resultado ---");
  console.log(`Atleta: ${nome}`);
  console.log(`Notas: ${notas.join(", ")}`);
  console.log(`Média: ${media.toFixed(2)}`);
}

// Executa
main();
