package br.senai.sp.roleta;

import java.util.Random;
import java.util.Scanner;

/**
 * Roleta Russa
 * Data 17/08/2023
 * Autor Franciel
 */

public class Roleta {
    public static void main(String[] args){
    /** Criar variaveis */
        int number;
        boolean continuar = true;
        int random;
        /**
         * Instancia scanner
         */
        Scanner teclado = new Scanner(System.in);


        Random aleatorio = new Random();

        while (continuar) {

            /** Coletar Dados do Usuario */
            System.out.println("/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/");
            System.out.println("-------- bem vindo  a Roleta ------");
            System.out.println("-------teste sua sorte --------");
            System.out.println("Digite um numero: ");
            number = teclado.nextInt();
            System.out.println("/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-");

            random = aleatorio.nextInt(10) + 1;
            if (random == number) {
                continuar = false;
            }
        }

    }
}
