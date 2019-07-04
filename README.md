# Task
task_ solution
// Разработайте программу, которая проверяет, что числа a, b и c различны (одинаковы).

public class Solution1 {
    int a;
    int b;
    int c;
    public static void main(String[] args) {
        System.out.println(var(3,5, 7));
        System.out.println(var(4,4,4 ));
    }
    public static boolean var(int a, int b, int c) {
        if (a == b && a == c)
            return true;
        return false;
       
    }
}

/*Масса динозавра задаётся в килограммах. Разработайте программу, которая вычисляет, сколько это миллиграмм, грамм и тонн.*/
public class Solution {

    public static void main(String[] args) {
        System.out.println(convertKgtoGramm(8));
        System.out.println(convertKgtoTon(1));
        System.out.println(convertKgtoMlg(3));
    }
        public static double convertKgtoGramm(double kg){
          double convertKgtoGramm = kg * 1000;
          return convertKgtoGramm;
    }
    public static double convertKgtoTon(double kg){
        double convertKgtoTon = kg/1000;
        return convertKgtoTon;
    }
    public static double convertKgtoMlg(double kg){
        double convertKgtoMlg = kg *1000000;
        return convertKgtoMlg;
    }
}
/*На плоскости даны два круга с общим центром и радиусами R1 и R2 (R1 > R2). Разработайте программу нахождения площади кольца, внешний радиус которого равен R1, а внутренний радиус равен R2.*/
public class Solution3_Circle {
    static double PI;
    static double R1;
    static double R2;
    public static void main(String[] args) {

        System.out.println(areaRing(3.1416, 10, 5));
    }
    public static double areaRing(double PI, double R1, double R2) {
   double s = PI* (Math.pow(R1, 2)- Math.pow(R2, 2));
        return  s;
    }
}

/*Написать программу, которая находит арифметическое и геометрическое среднее цифр шестизначного числа N.*/
public class Solution4 {
    public static void main(String[] args) {
        System.out.println(DigitsSorted(67397565));
    }
    public static boolean DigitsSorted (int k)
    {
        int m = k % 10;
        k /= 10;
        if (m == k % 10) return false;

        boolean abc = true;
        if (k % 10 > m) abc = false;
        while (k > 10) {
            m= k % 10;
             k/= 10;
            if (abc) {
                if (k  % 10 >= m) return false;
            } else {
                if ( k % 10 <= m) return false;
            }
        }
        return true;
    }
}
// Написать программу, которая переворачивает (реверсирует) семизначное число N (к примеру, число 1234567 реверсируется в число //7654321).

public class Solution6 {

    public static void main(String[] args) {
        StringBuffer rev = new StringBuffer("1234567");
        System.out.println(rev.reverse());
        }
    }
    public class Solution6 {

    public static void main(String[] args) {
        ArrayList<Integer> list = new ArrayList<>();
        for (int i = 1; i < 8; i++) {
            list.add(i);

        }
        for (int i = list.size() - 1; i >= 0; i--) {
            System.out.println(list.get(i));
        }
    }
}
/*Разработайте небольшую цельную программу, которая меняет местами содержимое двух целочисленных переменных a и b, не используя для этого дополнительных переменных*/
public class SwapAb {
   static int a ;
    static int b ;
    public static void main(String[] args) {
 
        System.out.println(swap(5, 6));
}
       public static int  swap(int a, int b) {
            return a;
        }
}

//Написать программу, которая находит арифметическое и геометрическое среднее цифр шестизначного числа N.

public class ArithmeticAndGeo {

    public static void main(String[] args) {
        System.out.println(ArithmeticAver(123456));
        System.out.println(GeometricAver(123456));
    }
        public static float ArithmeticAver (int a)
        {
            int sum = a % 10;
            int i = 1;
            while ( a > 10) {
                a /= 10;
                sum += a % 10;
                i++;
            }
            return sum / i;
        }

        public static double GeometricAver (int b)
        {
            int c = b % 10;
            int i = 1;
            while (b > 10) {
                b /= 10;
                c *= b % 10;
                i++;
            }
            return Math.pow(c, 1.0/i);
       }
}

  

    

