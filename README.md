package Introducao;

public class Aula04Operadores {
    public static void main(String[] args) {

        // + - / * Operadores Aritmeticos

        int numero01 = 10;
        int numero02 = 20;
        int resultado = numero01 / numero02; // será alocado em um terceiro lugar na memoria.

        //se colocar o + junto ao valor, valor será de concatenação e nao mais de soma.
        //exemplo abaixo
        System.out.println("Valor "+numero02+numero01); //Resultado será valor 2010 ao inves de 30 logo abaixo

        System.out.println(numero02+numero01); //Operação normal

        //porem se o valor estiver antes da String será feita a soma normalmente e depois concatenado
        System.out.println(numero01+numero02+" Valor");

        //resultado do terceiro elemento alocado na memoria

        System.out.println(resultado);

        // % resto

        int resto = 14 % 2;
        System.out.println(resto);

        //Operadores Relacionais

        // "< Menor"  "Maior >" "<= Menor igual"  "Maior igual=>" "== Comparação" "!= Diferente", esses operadores sempre vao retornar valores booleanos
        boolean isDezMaiorQueVinte = 10 > 20;
        boolean isDezMenorQueVinte = 10 < 20;
        boolean isDezIgualQueVinte = 10 == 20;
        boolean isDezDiferenteQueVinte = 10 != 20;
        System.out.println("isDezMaiorQueVinte? "+ isDezMaiorQueVinte);
        System.out.println("isDezMenorQueVinte? "+ isDezMenorQueVinte);
        System.out.println("isDezIgualQueVinte? "+ isDezIgualQueVinte);
        System.out.println("isDezDiferenteQueVinte? "+ isDezDiferenteQueVinte);

        //Operadores Lógicos
        // && (AND) || (OR) ! (NOT)
        int idade = 35;
        float salario = 3500F;

        boolean isDentroDaLeiMaiorQueTrinta = idade > 30 && salario >= 4612;
        boolean isDentroDaLeiMenorQueTrinta = idade < 30 && salario  >= 3381;
        System.out.println("isDentroDaLeiMaiorQueTrinta "+isDentroDaLeiMaiorQueTrinta);
        System.out.println("isDentroDaLeiMenorQueTrinta "+isDentroDaLeiMenorQueTrinta);

        double valorTotalContaCorrente = 200;
        double valorTotalContaPoupança = 10000;
        float valorPlaystation = 5000F;


        boolean isPlaystationCincoCompravel = valorTotalContaCorrente > valorPlaystation || valorTotalContaPoupança > valorPlaystation;
        System.out.println("isPlaystationCincoCompravel "+isPlaystationCincoCompravel);

        // Operadores de Atribuição
        // = += -= *= /= %=

        double bonus = 1800;
        bonus = bonus + 1000; //ou daria para fazer do mesmo jeito com +=
        System.out.println(bonus);

    }
}




package Introducao;

//Como dar um hello world e printar na tela

public class aula1HW {
    public  static void main(String[] args){
        System.out.println("Hello World");
    }
}


package Introducao;

public class aula2Comentarios {
    public static void main(String[] args){

        System.out.println("Preste Atenção nos tipos de comentarios");

        /**
         *  Isso é um comentário <b>javadoc</b>
         */

        // Isso é um comentario de uma Linha


        /*
            isso é um comentario de multiplas linhas
         */

        System.out.println("Não escreva comentarios obvios e bobos");
    }
}


package Introducao;


public class aula3TiposPrimitivos {
    public static void main(String[] args) {
        //int, double, float, char, byte, short, long, boolean
        int age = 10;
        double salarioDouble = 2000.0D;
        float salarioFloat = 2500F;
        byte idadeByte = 10;
        short idadeShort = 18;

        //exemplo de casting abaixo "força o valor de uma variavel na outra"
        long exemploCasting = (long) 155.98;

        // Casting não é muito bom estar utilizando! (Quase nunca)

        long numeroGrande = 10000000;
        boolean verdadeiro = true;
        boolean falso = false;
        char caractere = 65;


                // com a exceção do booelan todos os tipos acima são numéricos

        // String não é um tipo primitivo é uma CLASSE
        String nome = "Juliovsky";

        System.out.println("Oi meu nome é "+nome);
        System.out.println("A idade é "+age+" anos");
        System.out.println("char "+caractere);
        System.out.println(falso);
        System.out.println(exemploCasting);




    }
}



package Introducao;

/*
Prática
Crie variáveis para os campos descritos abaixo entre <> e imprima a seguinte mensagem:

Eu <nome>, morando no endereço <endereço>,
confirmo que recebi o salário de <salario>, na data <data>
 */


public class exercicio1 {
    public static void main(String[] args) {

        String nome = "Julio";
        String endereco = "Rua Catuipe, 289";
        double salario = 2311.67;
        String data = "23/12/2023";

        System.out.println("Eu " + nome + " morando no endereço, " + endereco + " confirmo que recebi o salário de " + salario + " na data " + data);

        // Outra forma seria colocando o resultado em uma String

        String nome2 = "Julio";
        String endereco2 = "Rua Catuipe, 289";
        double salario2 = 2411.67;
        String data2 = "24/12/2023";
        String relatorio = "Eu " + nome2 + " morando no endereço, " + endereco2 + " confirmo que recebi o salário de " + salario2 + " na data " + data2;
        System.out.println(relatorio);
    }
}



package Introducao;

public class aula0Facilidades {
    public static void main(String[] args) {
        System.out.println("Aqui estarão todas as facilidades para ser mais rapido na progrmação");
        //psvm = escreve rapidamente public static void main(String[] args)
        //sout = escreve rapidamente System.ou.println("Alguma coisa");
    }
}



package Introducao;
    public class biamar {
        public static void main(String[] args) {
            double salario = 2300.32;
            double aposentadoria = 1980.10;
            int idade = 20;
            float valorPlay7 = 7000;

            String nome = "pedro";
            String nome2 = "pedro2";
            boolean PlaystationCompravel = valorPlay7 < salario || valorPlay7 < aposentadoria;
            boolean PlaystationCompravel2 = nome == nome2;
            boolean resultado = PlaystationCompravel2 != PlaystationCompravel;
            System.out.println(resultado);

            //Tentar entender como funciona.

        }

}




