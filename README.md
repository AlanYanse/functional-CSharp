

# Gallery of example codes about functional programming.


![This is a alt text.](/image/book-functional-cisar.jpg)


## ForEach


```C#
List <string> names = new List <string>();

names.Add("Messi");

names.Add("Ronaldo");

names.Add("Modric´");

names.Add("Carlos Perciavale");


names.ForEach(p=>Console.WriteLine(p));
```

```C#
int[] intArray = new int[] {2, 3, 4};

Array.ForEach(intArray, p=>Console.WriteLine(p));
```

## Any

```C#
int[] intArray = new int[] {2, 3, 4};

bool exist = intArray.Any(p=>p == 3);

Console.WriteLine(exist);


//output

//true
```
## Map (Select)

```C#
List <int> listaNumeros = new List <int> {1,2,3,4};

List <int> squareNumeros = new List <int> (listaNumeros.Select(p=>p*p));

squareNumeros.ForEach(p=>Console.WriteLine(p));

//output

//1
//4
//9
//16
```

## LINQ
```C#
int[] arrayNumeros = new int[]{1,2,3,4,5,6,7,8,9,10};

List <int> numerosPares = new List <int>(from numero in arrayNumeros where numero % 2 == 0 select numero);

numerosPares.ForEach(p=>Console.WriteLine(p));

//output

//2
//4
//6
//8
//10
```
## OnHandleCreated (Click)
```C#
bt1.Click+=(s,e)=>{label1.Text = "i´m clicking";};

//output

//The Label1 show "i´m clicking".
```

## Func
```C#

using System;

class Program
{
    public static void Main(string[] args)
    {
   		
		int laSuma;

		Func<int, int, int>  Sum  = (x, y) => x + y;
		
		laSuma = Sum(10,5);

		Console.WriteLine(laSuma);


		
    }

	

}

//output

// 15
```

















