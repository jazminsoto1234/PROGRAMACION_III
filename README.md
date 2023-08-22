# PROGRAMACION_III

## TEMA 1 : FUNDAMENTOS DE PROGRAMACION

##### CONSTRUCTORES: 
Move constructor : El move constructor recibe como argumento el objeto del mismo tipo, pero una vez que realizar la asignacion, el objeto que se dio por parametro lo vacia usando nullptr.

POLIMORFISMO: Cuando un objeto se comporta diferente, sirve para generalizar.
SOBRECARGA DE OPERADORES : Se clasifican en 
* Numero de operandos : a++, --a, *a
* Unario: a + b
* Binario : cout<<y<<endl;
* Tercionario : condicion logica ternaria
* Con metodos

### SOBRECARGA BINARIA

Usando metodos : 
```cpp
vector<int> v1 = {10,20,30,40};
vector<int> v2 = {50,60,70};
auto v3 = v1<<v2 //{10,20,30,40,50,60,70};
auto v4 = v1 + v2 //{60,80,100,40};
// MAIN

auto v3 = concatenar(v1,v2);
auto v4 = sumarizar(v1,v2);
```

Usando sobrecarga:
```cpp
ostream& operator<<(ostream &o, const vector<int> &v2){
    for(const auto &item : v2){
        o<<item<<" ";
    }
    o<<endl;
    return o;
}
```

### SOBRECARGA DE OPERADOR UNARIO

Prefijo: Ambos mantienen el valor
```cpp
vector<int> operator++(const vector<int> &v1){
  for(int i=0; i<v1.size(); ++i){
    v1[i] = v1[i]++
  }
  return v1;
}
```

Subfijo : El primero devuelve lo mismo, luego el otro lo modifica
```cpp
vector<int>& operator++(const vector<int> &v1, int){
  for(auto const &item : v1){
    ++item;
  }
  return v1;
}
```




