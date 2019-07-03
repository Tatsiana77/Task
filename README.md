# Task
task_ solution
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
