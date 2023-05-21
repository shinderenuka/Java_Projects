# Java_Projects
public class Second_Largest_element {
    public static void main(String[] args) {
        int[] a = { 49, 35, 347, 16, 2 };
        int large = Integer.MIN_VALUE;
        int second_large = Integer.MIN_VALUE;
        for (int i = 0; i < a.length; i++) {
            if (a[i] > large) {
                second_large = large;
                large = a[i];
            } else if (a[i] > second_large && a[i] != large) {
                second_large = a[i];
            }
        }
        System.out.println("Largest element: " + large);
        System.out.println("Second largest element: " + second_large);
    }
}
