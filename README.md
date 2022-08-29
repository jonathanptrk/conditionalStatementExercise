# conditionalStatementExercise
Crie um algoritmo que receba os dados (nome e idade) digitados pelo usuário e identifique em qual categoria o atleta se encontra através da sua idade, imprima quando o atleta irá participar sendo:  

- De 7 até 14 categoria Infantil; 
- De 15 até os 17 categoria Juvenil; 
- De 18 até os 21 categoria Júnior; 
- de 22 até os 45 categoria Adulto;  

Infantil = Participa na segunda feira das 7h ás 12h; 
Juvenil = Participa na terça-feira das 9h ás 14h; 
Júnior = Participa na quarta-feira das 8h ás 13h; 
Adulto = Participa na quinta-feira das 18h ás 21h;

import java.util.Scanner;
public class EstruturasCondicionais {
    public static void main(String[] args) {

        System.out.println("Digite o seu nome completo: ");
        Scanner scan = new Scanner(System.in);
        String nomeAtleta = scan.nextLine().toUpperCase();

        System.out.println("Digite a sua idade: ");
        Scanner scan2 = new Scanner(System.in);
        int idadeAtleta = scan.nextInt();

        if(idadeAtleta > 6 && idadeAtleta <= 14 ){
            System.out.println("Nome: " + nomeAtleta);
            System.out.println("A sua idade: " + idadeAtleta);
            System.out.println("Você se enquadra na categoria: Infantil");
            System.out.println("Você participará na segunda-feira das 7h ás 12h");
        }else if (idadeAtleta > 14 && idadeAtleta <= 17){
            System.out.println("Nome: " + nomeAtleta);
            System.out.println("A sua idade: " + idadeAtleta);
            System.out.println("Você se enquadra na categoria: Juvenil");
            System.out.println("Você participará na terça-feira das 9h ás 14h");
        } else if (idadeAtleta > 17 && idadeAtleta <= 21) {
            System.out.println("Nome: " + nomeAtleta);
            System.out.println("A sua idade: " + idadeAtleta);
            System.out.println("Você se enquadra na categoria: Júnior");
            System.out.println("Você participará na quarta-feira das 8h ás 13h");
        } else if (idadeAtleta > 21) {
            System.out.println("Nome: " + nomeAtleta);
            System.out.println("A sua idade: " + idadeAtleta);
            System.out.println("Você se enquadra na categoria: Adulto");
            System.out.println("Você participará na quinta-feira das 18h ás 21h");
        } else {
            System.out.println("Não se enquadra em nenhuma das categorias disponíveis.");
        }
    }
}
