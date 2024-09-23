# Abstrakte Klasse
- werden mit dem Schlüsselwort `abstact`
deklariert.
- von abstrakten Klassen können **keine Objekte** erzeugt werden.
- sie dienen als Verwaltungsklassen in einer Vererbungshierarchie.

## Beispiel:

`````java
public abstract class Person{
    String name;
    String vorname;

    public Person(String name, String vorname){
        this.name = name;
        this.vorname = vorname;

    }

    public abstract boolean anmelden(String name, String kennwort);
}
`````

````java
public class Lehrer extends Person{
    
    public booloean anmelden(String name, String kennwort){

    }

public Lehrer(String name, String vorname){
    super(name,vorname);
}
}