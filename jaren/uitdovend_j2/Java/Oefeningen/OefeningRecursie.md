# Oefeningen Recursie

##1.1

### RaketCountDown
```java
public static void main(String[] args) {
    int counter = 6;
    RaketCountDown(counter);
}

public static int RaketCountDown(int timer){
    if (timer == 0) {
        System.out.println("Lift off");
        return 0;
    } else{
        System.out.println(timer);
        timer--;
    }
    return RaketCountDown(timer);
```

### Cijfers Tellen Recursief & iteratief

```java
public static void main(String[] args) {
    int eenGetal = 8008135;
    System.out.println(RecursiefCijfersTellen(eenGetal));
    System.out.println(IteratiefCijfersTellen(eenGetal));
}

public static int RecursiefCijfersTellen(int getal){
    if (getal == 0) {
        return 0;
    } return 1 + RecursiefCijfersTellen(getal/10);
}

public static int IteratiefCijfersTellen(int getal){
    int count = 0;
    while (getal > 0) {            
        getal /= 10;
        count++;
    }
    return count;
}
```
