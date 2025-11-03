import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int opcao = 0;

        while (opcao != 7) {
            System.out.println("=== SISTEMA DE CONTROLE DE DESPESAS ===");
            System.out.println("1 - Entrar Despesa");
            System.out.println("2 - Anotar Pagamento");
            System.out.println("3 - Listar Despesas em Aberto");
            System.out.println("4 - Listar Despesas Pagas");
            System.out.println("5 - Gerenciar Tipos de Despesa");
            System.out.println("6 - Gerenciar Usuários");
            System.out.println("7 - Sair");
            System.out.print("Escolha uma opção: ");

            opcao = sc.nextInt();
            sc.nextLine(); // Limpa buffer

            switch (opcao) {
                case 1:
                    System.out.println(">> Entrar Despesa selecionado");
                    break;
                case 2:
                    System.out.println(">> Anotar Pagamento selecionado");
                    break;
                case 3:
                    System.out.println(">> Listar Despesas em Aberto selecionado");
                    break;
                case 4:
                    System.out.println(">> Listar Despesas Pagas selecionado");
                    break;
                case 5:
                    System.out.println(">> Gerenciar Tipos de Despesa selecionado");
                    break;
                case 6:
                    System.out.println(">> Gerenciar Usuários selecionado");
                    break;
                case 7:
                    System.out.println(">> Saindo...");
                    break;
                default:
                    System.out.println("Opção inválida!");
            }
            System.out.println();
        }

        sc.close();
    }
}
