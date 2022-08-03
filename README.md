# Ejercicios-Tecnicos-Programador

// invertir una string

let text = "Mauricio Viana";
let textResult= "";

for (let i = text.length-1; i >= 0; i--) {
    textResult += text[i];
}

console.log(textResult);

//cuantas veces se repite un character

let string = "asdpoiasasdddddddAAADDDa088891assa";
let character = "a";
let contador = 0;

for (let c of string) {
    if (c === character) {
        contador++;
    }
}

console.log('el character %s se repite %i veces', character, contador);

//  Distancia de Hamming
//  comparar string con otra string
//  y contar cuantos caracteres son distinos

let string1 = "compukalaka";
let string2 = "compocasala";

let distancia = 0;

if string1.length != string2.length){
    console.log( strings de diferentes longitudes");
}
for (let i = 0; i < string1.length; i++) {
    if  string1[i] != string2[i]) {
        distancia++;
    }
}
console.log("Distancia es de: %i ",distancia);

// Contador de palabras

let string3 = "este string    contiene una      cantidad de words       "; string3 = string3.replace(/\s+/g, '/')
let words = 0;

for (let i = 0; i < string3.length; i++) {
    if string3[i] === '/'){
        words++;
    }
}

console.log string3 + '\nesta string contiene %i words',words);

//teniendo una string de caracteres contar cuantos números hay

let string3 = "as99111 264dfwerwe1r579qwe qw   e?asd1  a32 150   ";
let count =  string3.match(/[0-9]/g || [])).length;

console.log(count);
