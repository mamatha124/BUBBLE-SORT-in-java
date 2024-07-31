# BUBBLE-SORT-in-java
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
       Scanner sc=new Scanner(System.in);
        int l=sc.nextInt();
        int a[]=new int[l];
        System.out.print("Enter array: ");
        for(int i=0;i<l;i++){
            int k=sc.nextInt();
            a[i]=k;
        }
        for(int i=0;i<l;i++){
            for(int j=0;j<l-1;j++){
                if (a[j]>a[j+1]){
                    int t=a[j];
                    a[j]=a[j+1];
                    a[j+1]=t;
                }
            }
        }
        System.out.print("Array after sorting : ");
        for(int i=0;i<l;i++){
            System.out.print(a[i]+" ");
        }
    }
