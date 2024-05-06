
const vitorias = 85;
const derrotas = 20;
const resultado = calcularRanque(vitorias, derrotas);
console.log("Ranque do jogador: " + resultado);


// Função para calcular o ranque do jogador
function calcularRanque(vitorias, derrotas) {
    const saldo = vitorias - derrotas;
    let ranque;

    if (vitorias < 10) {
        ranque = "Ferro";
    } else if (vitorias >= 11 && vitorias <= 20) {
        ranque = "Bronze";
    } else if (vitorias >= 21 && vitorias <= 50) {
        ranque = "Prata";
    } else if (vitorias >= 51 && vitorias <= 80) {
        ranque = "Ouro";
    } else if (vitorias >= 81 && vitorias <= 90) {
        ranque = "Diamante";
    } else if (vitorias >= 91 && vitorias <= 100) {
        ranque = "Lendário";
    } else {
        ranque = "Imortal";
    }

    return ranque;
}
