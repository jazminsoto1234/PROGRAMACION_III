# PROGRAMACION_III

## TEMA 1 : FUNDAMENTOS DE PROGRAMACION

POLIMORFISMO: Cuando un objeto se comporta diferente, sirve para generalizar.
SOBRECARGA DE OPERADORES : Se clasifican en 
* Numero de operandos : a++, --a, *a
* Unario: a + b
* Binario : cout<<y<<endl;
* Tercionario : condicion logica ternaria
* Con metodos

  ### SOBRECARGA BINARIA
´´´cpp
vector<int> v1 = {10,20,30,40}
vector<int> v2 = {50,60,70}
auto v3 = v1<<v2 //{10,20,30,40,50,60,70}
auto v4 = v1 + v2 //{60,80,100,40}
// MAIN

auto v3 = concatenar(v1,v2)
auto v4 = sumarizar(v1,v2)

´´´
