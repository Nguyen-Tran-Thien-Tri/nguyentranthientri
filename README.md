# nguyentranthientri
import java.util.Scanner;
public class Lotto{
 public static void main(String[] args){
  Scanner number= new Scanner(System.in);
  System.out.println("Many game : ");
  int many = number.nextInt();
  int min =1;
  int max =49;
  int a=0;
  int b=0;
 for(int j=0;j<many;j++){
 for(int i=0;i<6;i++){
 int random_int =(int)(Math.random() * (max-min)+1);
if(random_int== 11 | random_int== 43 |random_int == 24|random_int==30|random_int==48|random_int==35)
{a=a+1;}
  System.out.println(random_int);}
   if(a==1|a==2){
   System.out.println("you have $10");
   b=b+10;
  }
  else if(a==3){
  System.out.println("you have $100");
  b=b+100;
}
 else if(a==4){
  System.out.println("you have $1000");
  b=b+1000;
}
 else if(a==5){
  System.out.println("you have $5000");
  b=b+5000;
}
 else if(a==6){
  System.out.println("you have $5 million");
  b=b+5000000;
}
 else if(a==0){
   System.out.println("you are loss");
 b=b;
}
}
  System.out.print("Total money won : ");
  System.out.println(b);
  System.out.println("Total tiket cost : ");
  System.out.println(4*many);
  System.out.println("Profit/loss : ");
  System.out.print(b-4*many);
}}
