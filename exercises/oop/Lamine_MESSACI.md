# [Exercises] OOP_Lamine MESSACI

<img src="../../art/oclogo.png" alt="drawing" width="150"/>

## Cet exercice a pour but la maitrise des bases de la programmation objet en JAVA

### Ennonc� :

1 - Cr�er une classe CarBrand (marque de voiture) avec les attributs suivants :

� name (String)
� address (String)
```

```
R�pondre ici


public class CarBrand{

	private String name;
	private String address;
}

2 -  Cr�er une classe Car (voiture) avec les attributs suivants :

```
� name (String)
� color (String)
� kilometers (int)
� brand (CarBrand)
```

```
R�pondre ici

public abstract class  Car {
	private String name;
	private String color;
	private int kilometers;
	private CarBrand brand;
}

3 - Cr�er un constructeur pour les 2 classes qui initialise toutes les propri�t�s de la classe.

```
R�pondre ici
 
 public CarBrand (String name, String address){

 	this.name = name;
 	this.adress = address;
 }

 public CarBrand(String name) {
        this.name = name;
    }

public Car(String name, String color, int kilometers, CarBrand brand){

    this.name =name;
    this.color = color;
    this.kilometers = kilometers;
    this.brand = brand;

}

  public Car(String name) {
        this.name = name;
    }

4 - Cr�er 2 objets "marque de voitures" (Renault et Citro�n).


R�pondre ici
...

5 - Cr�er 3 objets "voiture" (Clio, Twingo et Saxo) avec leurs marques associ�es.

```
R�pondre ici

        Voiture clio = new Voiture("Clio");
        Voiture twingo = new Voiture("Twingo");
        Voiture saxo = new Voiture("Saxo");

6 - Ajouter 1 m�thode "start" sur la classe "Car" qui affiche le nom de la voiture et "vrooom" dans la console.

```
R�pondre ici

protected abstract void star();

7 - Appeler la m�thode "start" sur la Clio et la Twingo.

```
R�pondre ici

 @Override
    protected void star() {
        System.out.println(this.getName()+ " Vroom!!");
    }

8 - Le programme doit afficher "Clio vrooom" et "Twingo vrooom" dans la console.

```
R�pondre ici

        clio.star();
        twingo.star();
        saxo.star();


