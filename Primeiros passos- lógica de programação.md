# Primeiros passos na lógica de programação





<meta charset="UTF-8">


<script>

    function pulaLinha() {
    
        document.write("<br>");
        document.write("<br>");
}

    function mostra(frase) {
    
        document.write(frase);
        pulaLinha();
}

    function calculaImc(altura, peso) {
    
        return peso / (altura * altura);
}

var nome = prompt("Informe o seu nome");
var alturaInformada = prompt(nome + ", informe sua altura");
var pesoInformado = prompt(nome + ", informe seu peso");

var imc = calculaImc(alturaInformada, pesoInformado);

if(imc < 18.5) {

    mostra("Você está abaixo do recomendado");

}

if(imc > 24.9) {

    mostra("Você está acima do recomendado");
}

if(imc >= 18.5) {

    if(imc <= 24.9) {
    
        mostra("Seu IMC está excelente!");
    
    }

}

mostra (nome + ", o seu IMC é " +  imc);

</script>

Ref: Curso de Lógica de programação I - Alura