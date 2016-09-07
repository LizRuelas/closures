+++Codigo Inicial

var num2 = 0;

function suma(num1) {
	return function() {
		return num1 + num2;
	}
} 

var suma2 = suma(2);
console.log(suma2(5)); 

var suma12 = suma(12);
console.log(suma12(76));


+++Codigo Modificado

var num2 = 0;

function suma(num1) {
	return function(num2) {
		return num1 + num2;
	}
} 


var suma2 = suma(2);
console.log(suma2(5)); 

var suma12 = suma(12);
console.log(suma12(76));

explicacion: en la linea 6 no esta pasandose el parametro de la varible num2 es decir en el return no usa el num2 porque 
es como si no existiera al colocar el parametro recien lo reconoce e imprime correctamente.
