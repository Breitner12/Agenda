## Evidencias realizadas
registros de notas

## Hoja de vida

aprendimos a realizar una hoja de vida con markdown

[hoja de vida] (https://github.com/Breitner12/Hoja-de-vida.git)

## Visual Basic

se aprendio a ponerle el valor a la variable.

<a href="https://ibb.co/phHWY68"><img src="https://i.ibb.co/fD38jV5/visual-basic.png" alt="visual-basic" border="0"></a>

## StarUMTL

en starUMTL la variable se usa en un rectangulo.

<a href="https://ibb.co/WfSHBnM"><img src="https://i.ibb.co/hVpg2s4/strauml.png" alt="strauml" border="0"></a>


## Algoritmo 

<a href="https://ibb.co/WfSHBnM"><![image](https://user-images.githubusercontent.com/110871046/186992597-202a63ac-a429-4fce-b16f-e16c07db776e.png)></a>

## Ejercicio mientras que

~~~
Sub prueba()
   c = 0
   b = 0
   nb = 0
   a = 0
   t = 0
      While t < 3000000
         c = Int(InputBox("ingrese la cantidad: "))
         If c >= 1 Then
            b = b + 1
         End If
         If c >= 10000 Then
            a = a + 1
         End If
         If c <= o Then
            nb = nb + 1
         End If
            t = t + c
      Wend
      promedio = (t / b)
      MsgBox ("abonaron: " & b)
      MsgBox ("abonaron10k: " & a)
      MsgBox ("no abonaron: " & nb)
      MsgBox ("total recaudado: " & t)
      MsgBox ("promedio los que aportaron: " & promedio)
End Sub
~~~

## Ejercicio busqueda

~~~
Sub ejercicio()
    contador = m.Cells(1, 6)
    sw = True
    cedula = Int(InputBox("ingrese su ID: "))
    While sw
        If cedula = m.Cells(contador, 1) Then
            n = m.Cells(contador, 2)
            sw = False
            MsgBox " el nombre es:" & n
        End If
        If x = 20 Then
            MsgBox " no hay resultados"
            sw = False
        End If
        contador = contador + 1
    Wend
End Sub
~~~
## Formulario visual basic

~~~
Private Sub btneliminar_Click()
 
  actual = Hoja1.Cells(2, 6)
  Hoja1.Rows(actual).EntireRow.Delete
  TXTnombre.Text = Empty
  TXTid.Text = Empty
  TXTcelular.Text = Empty
  COMsexo.Text = Empty
  Hoja1.Cells(1, 6) = Hoja1.Cells(1, 6) - 1
  
  
End Sub

Private Sub CMDguardar_Click()
   
   Worksheets("base de datos").Range("A2").EntireRow.Insert
   Range("A2") = TXTid.Value
   Range("B2") = TXTnombre.Value
   Range("C2") = TXTcelular.Value
   Range("D2") = COMsexo.Value
   
   TXTid = Empty
   TXTnombre = Empty
   TXTcelular = Empty
   COMsexo = Empty
   Hoja1.Cells(1, 6) = Hoja1.Cells(1, 6) + 1
   com = Hoja1.Cells(2, 6)
   
End Sub


Private Sub COMbuscar_Click()
    fila = 2
    com = Hoja1.Cells(2, 6)
    sw = True
    While sw
        
        If Hoja1.Cells(fila, 1) = TXTid.Text Then
            
            TXTnombre.Text = Hoja1.Cells(fila, 2)
            TXTcelular.Text = Hoja1.Cells(fila, 3)
            COMsexo.Text = Hoja1.Cells(fila, 4)
            sw = False
        Else
           
           If Hoja1.Cells(2, 1) = "" Then
                MsgBox "no se encontro nada"
                sw = False
           End If
        End If
            fila = fila + 1
            com = com + 1
    Wend
        fila = fila - 1
        Hoja1.Cells(2, 6) = fila
         
                     
    
End Sub

Private Sub COMeditar_Click()
       
    
    TXTnombre.Enabled = True
    TXTid.Enabled = False
    TXTcelular.Enabled = True
    COMsexo.Enabled = True
    TXTnombre.SetFocus
    CMDguardar.Enabled = True
    COMbuscar.Enabled = False
    COMeditar.Enabled = False
    
    
        
End Sub

Private Sub COMnuevo_Click()

     frm_ingreso.Caption = "nuevo registro"
     TXTnombre.Enabled = False
     TXTid.Enabled = True
     TXTcelular.Enabled = True
     COMsexo.Enabled = True
     TXTnombre.Text = Empty
     TXTid.Text = Empty
     TXTcelular.Text = Empty
     COMsexo.Text = Empty
     CMDguardar.Enabled = True
     COMbuscar.Enabled = False
     COMeditar.Enabled = False
     TXTid.SetFocus
     Hoja1.Cells(1, 6) = Hoja1.Cells(1, 6) + 1
     Hoja1.Cells(2, 6) = Hoja1.Cells(1, 6)
     
     
     
End Sub

Private Sub UserForm_Initialize()
   COMsexo.List = Worksheets("lista").Range("A2:A3").Value
   
End Sub
~~~

## Ejercicio de dartpad
~~~

void main() {
  Operacion operacion = new Operacion();

  operacion.num1 = 3.4;
  operacion.num2 = 5.7;

  print(operacion.sumar());
  operacion.resta();
  print(operacion.multi());
}

class Operacion {
  double? num1;
  double? num2;

  double sumar() {
    double m = num1! + num2!;
    return m;
  }

  void resta() {
    double r = num1! - num2!;
    print(r);
  }

  double multi() {
    double mul = num1! * num2!;
    return mul;
  }
}
~~~

## Ejercicio 2  de dartpad

~~~
void main() {
  Person person = new Person(s: "Masculino", n: "jaime ");

  person.nombre = "jaime";
  person.apellido = "Mora";
  person.edad = 45;
  person.sexo = "Masculino";
  print('su nombre completo es:${person.nombreCompleto()}');
  person.edadMas(person.edad);
  print('su sexo es:${person.sexo}');
}

class Person {
  String? nombre;
  String? sexo;
  String? apellido;
  int? edad;

  Person({String? n, String? s}) {
    nombre = n;
    sexo = s;
  }
  String nombreCompleto() {
    String? n = nombre! + " " + apellido!;
    return n;
  }

  void edadMas(p) {
    int s = p + 5;
    print('su edad es: $s ' 'años');
  }
}
~~~

## Constructor en dartpad

~~~

void main() {
  Person person = new Person(s: "Masculino", n: "jaime ");

  person.nombre = "jaime";
  person.apellido = "Mora";
  person.edad = 45;
  person.sexo = "Masculino";
  print('su nombre completo es:${person.nombreCompleto()}');
  person.edadMas(person.edad);
  print('su sexo es:${person.sexo}');
}

class Person {
  String? nombre;
  String? sexo;
  String? apellido;
  int? edad;

  Person({String? n, String? s}) {
    nombre = n;
    sexo = s;
  }
  String nombreCompleto() {
    String? n = nombre! + " " + apellido!;
    return n;
  }

  void edadMas(p) {
    int s = p + 5;
    print('su edad es: $s ' 'años');
  }
}
~~~

## Herencia dartpad

~~~

void main() {
  Leon leon = new Leon();
  leon.edad = 55;
  leon.habitad = "africa";
  leon.especie = "depredador";
  leon.carne = "gasela";
  Conejo conejo = new Conejo();
  conejo.especie = "herbivoro";
  conejo.edad = 22;
  conejo.habitad = "sudamerica";
  Hiena hiena = new Hiena();
  hiena.especie = "depredador";
  hiena.edad = 55;
  hiena.habitad = "africa";
  Hombre hombre = new Hombre();
  hombre.edad = 89;
  hombre.especie = "humana";
  hombre.habitad = "cualquiera";

  print(
      'la especie es: ${leon.especie},su edad es: ${leon.edad} y su comida favorita es la ${leon.carne}');
  (leon.edad);
}

class Animal {
  String? especie;
  int? edad;
  String? habitad;
}

class Omnivoro extends Animal {}

String? detodito;

class Carnivoro extends Animal {
  String? carne;
}

class Herbivoro extends Animal {
  String? frutas;
}

class Conejo extends Herbivoro {}

class Leon extends Carnivoro {}

class Hiena extends Carnivoro {}

class Hombre extends Omnivoro {}

~~~

## Metodo string dartpad

~~~

void main() {
  List lista = ["colombia", "peru", "alemania"];
  List hoja = [11444, 32324, 12131];
  List docu = ["este", "norte", "oeste"];
  for (int i = 0; i < 3; i++) {
    Empresa empresa =
        new Empresa(pais: lista[i], numero: hoja[i], oficina: docu[i]);

    print(empresa.generalCodigo());
  }
}

class Empresa {
  String? pais;
  int? numero;
  String? oficina;

  Empresa({this.pais, this.numero, this.oficina});

  String? generalCodigo() {
    String p = pais!.substring(1, 3);
    int ope = oficina!.length;
    int ofi = ope - 3;
    String? ofici = oficina!.substring(ofi, ope);
    String? pasar = numero.toString();
    String numeros = pasar.substring(2, 3);
    return "$p$numeros$ofici";
  }

  void cantCaracteres() {
    int p = pais!.length;
    int ofici = oficina!.length;
    String? pasar = numero!.toString();
  }
}

~~~

## User

~~~

import 'dart:convert' as convert;

class User {
  String? nombre;
  String? avatar;
  String? email;

  User(String json) {
    final JsonResponse = convert.jsonDecode(json);
    nombre = JsonResponse["data"]["first_name"];
    avatar = JsonResponse["data"]["avatar"];
    email = JsonResponse["data"]["email"];
  }
}
~~~

## Template

~~~
import 'package:flutter/material.dart';
import '../models/user.dart';

class Template extends StatelessWidget {
  const Template({
    Key? key,
    required this.user,
  }) : super(key: key);
  final User user;
  @override
  Widget build(BuildContext context) {
    return Column(
      children: [
        SizedBox(height: 15.0),
        Text(
          user.nombre!,
          style: TextStyle(fontSize: 25.0),
        ),
        Image(
          image: NetworkImage(user.avatar!, scale: 1.0),
        ),
        Text(
          user.email!,
          style: TextStyle(fontSize: 17.0, fontStyle: FontStyle.italic),
        ),
        Row(
          mainAxisAlignment: MainAxisAlignment.spaceEvenly,
          children: [
            Icon(
              Icons.email,
              color: Colors.red,
              size: 34.0,
            ),
            Icon(
              Icons.facebook,
              color: Colors.blue,
              size: 35.0,
            ),
            Icon(
              Icons.whatshot_sharp,
              color: Colors.blue,
              size: 36.0,
            ),
          ],
        )
      ],
    );
  }
}
~~~

## Main

~~~
import 'package:flutter/material.dart';
import 'models/user.dart';
import 'package:http/http.dart' as http;
import 'widgets/template.dart';

void main() => runApp(Sena());

class Sena extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Sena',
      home: Scaffold(
          appBar: AppBar(
            title: Text('my app'),
          ),
          body: FutureBuilder<User>(
            future: getUser(),
            builder: (context, snapshot) {
              if (snapshot.connectionState == ConnectionState.done) {
                User user = snapshot.data as User;
                return Template(user: user);
              }
              return Center(child: CircularProgressIndicator());
            },
          )),
    );
  }

  Future<User> getUser() async {
    final url = Uri.https('reqres.in', '/api/users/10');
    final response = await http.get(url);
    return User(response.body);
  }
}
~~~

