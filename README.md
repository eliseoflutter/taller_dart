![dart](https://www.dartlang.org/assets/shared/dart-logo-for-shares.png?2)

# Taller de Dart

*Este taller de dart es impulsado por la meta-comunidad de [FlossPA](https://floss-pa.net/) y dirigido por [Harry Alvarado](https://github.com/HarryAlvarado28).*

## Objetivos
Aprender ¿qué es Dart? su potencial y sintaxis.

## Concepto

**Dart** es un lenguaje optimizado por el cliente para aplicaciones rápidas en cualquier plataforma.

Potencial
- Optimizadopara UI
- Desarrollo productivo
- Rápido en todas las plataformas

```dart
/* Hola mundo en Dart */
main() {
  print("Hola, Mundo!");
}
```

## Contenido

### Palabras reservadas
![palabras-reservada](Palabras-Reservadas.png)

### Tipo de datos

- Números *(int, double)*
- Strings
- Booleans
- List
- Sets
- Maps

### Ejemplos de Tipo de datos

#### Números *(int, double)*

```dart
void main() {
// Numeros
  int a = 12;
  double b = 12.5;
  int c = a + 5;
  
  print(a);
  print(b);
  print(c);
    
  // Tambien ser permite
  int _d = 5;
  double $e = 5.4;
  print(_d);
  print($e);  
}
```

#### Strings

```dart
void main() {
// Strings - cadena de caracteres
  String nombre = 'Harry';
  String nombre2 = "Harry";
  String nombre3 = 'Harry\'s';
  
  print(nombre);
  print(nombre2);
  print(nombre3);
  
  String multilinea = '''Cuando se quieres hacer una variable que contenga multiples lineas se debe colocar tres comillas simples al principio de la cadena de caracteres y tres al final.''';
  
  print(multilinea);
  
}
```

#### Booleans

```dart
void main() {
// Booleans
  bool activo = true;
  bool vivo = false; 

  vivo = !vivo;
  
  print(activo);
  print(vivo);
}
```


#### List - Arreglos

```dart
void main() {
  // Listas - Arreglos
  
  // Listas Dinamicas
  List loquesea = ['Superman', 'Ironman', 10, true];
  print(loquesea);
  
  List<String> heroes = ['Capitan America', 'Deadpool'];
  heroes.add('Batman');
  print(heroes);
  
  List<int> miles = [2000, 2001, 2018, 2019];
  print(miles);
  
  List<double> valores_math = new List();
  valores_math..add(3.14)..add(2.71)..add(1.61);
  print(valores_math);
  
  
  // Listas estaticas
  List<String> frutas = new List(3);
  frutas[0] = 'Manzana';
  //frutas[1] = 'Uvas';
  frutas[2] = 'Piña';
  
  print(frutas);    
}
```

#### Set - *(similar a las listas)*

```dart
void main() {
  // Set  
  Set loquesea = {'Superman', 'Ironman', 10, true};
  loquesea.add('Superman');
  print(loquesea);
  
  Set<String> heroes = {'Capitan America', 'Deadpool'};
  heroes.add('Batman');
  heroes.add('Deadpool');
  print(heroes);
  
  Set<int> miles = {2000, 2001, 2018, 2019};
  miles.add(2018);
  print(miles);
  
  Set<double> valores_math = new Set();
  valores_math..add(3.14)..add(2.71)..add(1.61);
  print(valores_math);
}
```

*La principal diferencia entre los **List** y los **Set**, consiste en que no puedes agregar un valor repetido, a la Set.*

#### Maps

```dart
void main() {
  // Maps
  var loquesea = {
    'letra': 'a',
    'numero': 7,
    14000:'catorce mil',
    'activo': true
  };
  
  print(loquesea);
  print(loquesea['numero']);
  
  Map<double, String> constantes_matematicas  = {
    3.14:'PI',
    2.71:'Constante de Napier',
    1.61:'Número áureo'
  };
  
  constantes_matematicas.addAll({-2.50:'Constante α de Feigenbaum'});
  print(constantes_matematicas);
  print(constantes_matematicas[2.71]);
  
  Map<String, dynamic> Panama = new Map();
  Panama.addAll({
    'capital': 'Panamá',
    'telefono': 507,
    'superficie': 75.517,
    'moneda': 'Dólar estadounidense, Balboa',
  });
  print(Panama);
  print(Panama['superficie']);
}
```

