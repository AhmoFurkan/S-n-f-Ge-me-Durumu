# S-n-f-Ge-me-Durumu
Eğer girilen ders notları 0 veya 100 arasında değil ise hesablanmaz


    import java.util.Scanner;

    public class Main {

    public static void main(String[] args) {
        int Matematik, Fizik, Türkçe, Kimya, Müzik;
        Scanner inp = new Scanner(System.in);


        System.out.print("Matematik notunuz :");
        Matematik = inp.nextInt();
        if (Matematik > 0 && Matematik < 100) {


            System.out.print("Fizik notunuz :");
            Fizik = inp.nextInt();
            if (Fizik > 0 && Fizik < 100) {


                System.out.print("Türkçe notunuz :");
                Türkçe = inp.nextInt();
                if (Türkçe > 0 && Türkçe < 100) {


                    System.out.print("Kimya notunuz :");
                    Kimya = inp.nextInt();
                    if (Kimya > 0 && Kimya < 100) {


                        System.out.print("Müzik notunuz :");
                        Müzik = inp.nextInt();
                        if (Müzik > 0 && Müzik < 100) {


                            double avarage = (Matematik + Türkçe + Fizik + Müzik + Kimya) / 5.0;
                            if (avarage >= 55) {
                                System.out.println("Geçtiniz ! :" + avarage);
                            } else if (avarage < 55) {
                                System.out.println("Kaldınız !" + avarage);
                            }
                        }
                    }

                }

            }

        }
        System.out.println("Hesablanmaz");


    }

}
