# Link-list-program
/**a program that can store 10 records of students in a link list manner and apply the following operations on it. View the list ,Insert the elements in different locations of linked list and view it. Search any element from the linked list.Delete record again view the list after deletion. 
*/
package com.company;
import java.util.Arrays;
public class Main {
    public static void main(String[] args) {
        String[] names = {"Mukadus", "Abdullah", "Nofil", "Rabee", "Ibrahim", "Malik", "Ramna", "Mahnoor", "Rafay", "Inshal"};
        int[] id = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
        double[] salary = {36436, 37527, 9874, 38747, 37237, 128147, 182743, 82943, 84937, 4738};
        System.out.println("VIEWING THE LIST : ");
        System.out.println();
        System.out.println("ID: " + id[0] + "," + "NAME: " + names[0] + "," + "SALARY: " + salary[0]);
        System.out.println("ID: " + id[1] + "," + "NAME: " + names[1] + "," + "SALARY: " + salary[1]);
        System.out.println("ID: " + id[2] + "," + "NAME: " + names[2] + "," + "SALARY: " + salary[2]);
        System.out.println("ID: " + id[3] + "," + "NAME: " + names[3] + "," + "SALARY: " + salary[3]);
        System.out.println("ID: " + id[4] + "," + "NAME: " + names[4] + "," + "SALARY: " + salary[4]);
        System.out.println("ID: " + id[5] + "," + "NAME: " + names[5] + "," + "SALARY: " + salary[5]);
        System.out.println("ID: " + id[6] + "," + "NAME: " + names[6] + "," + "SALARY: " + salary[6]);
        System.out.println("ID: " + id[7] + "," + "NAME: " + names[7] + "," + "SALARY: " + salary[7]);
        System.out.println("ID: " + id[8] + "," + "NAME: " + names[8] + "," + "SALARY: " + salary[8]);
        System.out.println("ID: " + id[9] + "," + "NAME: " + names[9] + "," + "SALARY: " + salary[9]);
        System.out.println();
        //////////////////////////////////////
        System.out.println("INSERTION : ");
        System.out.println();
        int Index_position1 = 9;
        int newValue1 = 10;
        id[Index_position1] = newValue1;
        int Index_position = 9;
        String newValue = "Saleem";
        names[Index_position] = newValue;
        int Index_position2 = 9;
        int newValue2 = 546454;
        salary[Index_position2] = newValue2;
        System.out.println("NEW ARRAY : " + Arrays.toString(id));
        System.out.println();
        System.out.println("NEW ARRAY : " + Arrays.toString(names));
        System.out.println();
        System.out.println("NEW ARRAY : " + Arrays.toString(salary));
        System.out.println();
        ////////////////////////////////////////
        System.out.println("DELETION : ");
        int[] arr_new = new int[id.length - 1];
        int j = 9;
        for (int i = 0, k = 0; i < id.length; i++) {
            if (i != j) {
                arr_new[k] = id[i];
                k++;
            }
        }
        String[] arr_new1 = new String[names.length - 1];
        int l = 9;
        for (int i = 0, m = 0; i < names.length; i++) {
            if (i != l) {
                arr_new1[m] = names[i];
                m++;
            }
        }
        System.out.println();
        System.out.println("Before deletion :" + Arrays.toString(id));
        System.out.println("After deletion :" + Arrays.toString(arr_new));
        System.out.println();
        System.out.println("Before deletion :" + Arrays.toString(names));
        System.out.println("After deletion :" + Arrays.toString(arr_new1));
        System.out.println();
        System.out.println("Before deletion :" + Arrays.toString(salary));
        System.out.println("After deletion :" + Arrays.toString(arr_new2));
        System.out.println();
        System.out.println("SEARCHING : ");
        boolean found = false;
        int index = 0;
        String s = "Mukadus";
        for (int i = 0; i < names.length; i++) {
            if(s.equals(names[i])) {
                index = i; found = true; break;
            }
        }
        if(found)
            System.out.println(s +" found at the index "+index);
        else
            System.out.println(s +" not found in the array");
    }
}
        

