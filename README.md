import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        System.out.println("=== PROYECTO LISTAS ===");

        List<Integer> numeros = new ArrayList<>();
        numeros.add(10);
        numeros.add(20);
        numeros.add(30);
        numeros.add(40);
        numeros.add(50);
        numeros.add(60);

        System.out.println("Lista de números: " + numeros);

        int suma = 0;
        for (int numero : numeros) {
            suma += numero;
        }
        System.out.println("Suma total: " + suma);

        List<String> nombres = new ArrayList<>();
        nombres.add("Ana");
        nombres.add("Carlos");
        nombres.add("María");
        nombres.add("Juan");
        nombres.add("Laura");
        nombres.add("Pedro");

        System.out.println("\n=== IMPRESIÓN DE NOMBRES ===");

        System.out.println("\nUsando for:");
        for (int i = 0; i < nombres.size(); i++) {
            System.out.println((i + 1) + ". " + nombres.get(i));
        }

        System.out.println("\nUsando foreach:");
        int contador = 1;
        for (String nombre : nombres) {
            System.out.println(contador + ". " + nombre);
            contador++;
        }

        System.out.println("\nUsando while:");
        int index = 0;
        while (index < nombres.size()) {
            System.out.println((index + 1) + ". " + nombres.get(index));
            index++;
        }
    }
}
