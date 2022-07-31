# shorting-of-array
import java .util.Scanner;
public class INTRO {
    public static void main(String[] args) {
        int temp;
        Scanner sc=new Scanner(System.in);
        System.out.println("enter the size of n array");
        int size=sc.nextInt();
        int array[]=new int [size];

        // loop for taking input
        System.out.println("enter the element in array");
        for (int i=0;i<size;i++){
            array[i]=sc.nextInt();
        }

        // for output
        System.out.println("the existing array is");
        for (int i=0;i<size;i++){
            System.out.println(array[i]);
        }
// this is program for shorting
        // loop for traversing on array
        for (int i=0;i<size-1;i++){
            // loop for comparing
            for (int j=0;j<size-1 ;j++){
                if (array[j]>array[j+1]){
                    temp=array[j];
                    array[j]=array[j+1];
                    array[j+1]=temp;

                }
            }

        }
        System.out.println("the array after shorting");
       for (int i=0;i<size;i++){
           System.out.println(array[i]);
       }

        



    }
}
