## Evidencias realizadas
registros de notas

## hoja de vida

aprendimos a realizar una hoja de vida con markdown

[hoja de vida] (https://github.com/Breitner12/Hoja-de-vida.git)

## visual Basic

se aprendio a ponerle el valor a la variable.

<a href="https://ibb.co/phHWY68"><img src="https://i.ibb.co/fD38jV5/visual-basic.png" alt="visual-basic" border="0"></a>

## starUMTL

en starUMTL la variable se usa en un rectangulo.

<a href="https://ibb.co/WfSHBnM"><img src="https://i.ibb.co/hVpg2s4/strauml.png" alt="strauml" border="0"></a>


## algoritmo

<a href="https://ibb.co/WfSHBnM"><![image](https://user-images.githubusercontent.com/110871046/186992597-202a63ac-a429-4fce-b16f-e16c07db776e.png)></a>

## ejercicio mientras que

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

## ejercicio busqueda

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

## ejercicio 2 dart

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
