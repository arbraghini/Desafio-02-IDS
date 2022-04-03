# Desafio-02-IDS
Programa de seleção da empresa IDS
Programa para mostrar todos os numeros n menores que 10.000, onde n e n + 1 possuem o mesmo número de divisores.

====================================================================================

Passos para executar o programa em Java.
 1 - Salve o arquivo o programa em alguma Pasta do Windows.
 2 - Clique no botão Iniciar e digite cmd. Pressione ↵ Enter para abrir o "Prompt de Comando".
 3 - Verifique se o Java está instalado. Digite java -version na linha de comando. Se o Java estiver instalado, você verá uma mensagem mostrando qual a versão dele            está instalada. Se isso não acontecer, será necessário acessar o site do Java e baixar o Java Development Kit (JDK), que é gratuito e pode ser encontrado aqui:          http://www.oracle.com/technetwork/java/javase/downloads/index.html.
 4 - Vá até a pasta correta. Use o comando cd seguido pelo nome da pasta de destino para sair do diretório atual.
     Por exemplo, se você estiver no diretório C:\Users\Bob\Project e quiser acessar a pasta C:\Users\Bob\Project\TitanProject , digite cd TitanProject e pressione ↵          Enter. Para mostrar uma lista com todos os arquivos e pastas do diretório atual, digite dir no Windows ou ls no Mac e pressione ↵ Enter
 5 - Execute o programa. Digite java arquivo e pressione ↵ Enter. Lembre-se de que você deve trocar "arquivo" pelo nome do arquivo do seu programa.
     Após pressionar ↵ Enter, o programa deve rodar.
     
 ======================================================================================= 
  
  Tecnologias utilizadas:
  1 - Java\jdk1.8.0_311
  2 - Prompt de Comando do DOS.
  3 - Bloco de Notas
     
=======================================================================================
     
public class NumDivisor
{
	public static void main( String args[])
	{	
	int num;
	 for ( int n = 1; n <=10000; n++)
	   {  
	    int x=1;
	    int y=1;
	    int contx = 0;
	    int conty = 0;
	    num = n;	
	    while (x < 10000){
	      if (n % x == 0) 
	      contx++;
		x++;
	     }
		num++;
		while (y < 10000){
		if ( num % y == 0)
		  conty++;
		  y++;
	      }
	    if (contx == conty )
	    System.out.println("" + n + " " + num + " " + contx + " " + conty + "");
	   }
	}
}
