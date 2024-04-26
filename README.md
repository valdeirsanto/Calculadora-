import java.util.Scanner;

  public class calculadora  {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        double num1, num2;
        System.out.println("Digite o primeiro número: ");
        num1 = input.nextDouble();
        System.out.println("Digite o segundo número: ");
        num2 = input.nextDouble();

        System.out.println("Escolha a operação desejada: ");
        System.out.println("1 - Adição");
        System.out.println("2 - Subtração");
        System.out.println("3 - Multiplicação");
        System.out.println("4 - Divisão");

        int op = input.nextInt();

        switch(op) {
            case 1:
                System.out.println("Resultado: " + (num1 + num2));
                break;
            case 2:
                System.out.println("Resultado: " + (num1 - num2));
                break;
            case 3:
                System.out.println("Resultado: " + (num1 * num2));
                break;
            case 4:
                if (num2 != 0) {
                    System.out.println("Resultado: " + (num1 / num2));
                } else {
                    System.out.println("Não é possível dividir por zero.");
                }
                break;
            default:
                System.out.println("Opção inválida.");
        }
    }
}
