using System;

namespace COVID19_TANI_PROGRAMI
{
    class Program
    {
        static void Main(string[] args)
        {
            string isim, soyad, yas, şehir, ates, nefesdarlıgı, öksürük;
            Console.Title = "COVID-19 TANI PROGRAMI";//Konsol uygulamasının başlığını düzenler.
            Console.ForegroundColor = ConsoleColor.Yellow;

            Console.WriteLine("İsminizi Giriniz "); //Ekrana yazı yazdırma metodu.
            isim = Console.ReadLine(); //Klavyeden girilen değeri isim değişkenine atar.
            Console.WriteLine("Soyadınızı Giriniz ");
            soyad = Console.ReadLine();
            Console.WriteLine("Yaşınızı Giriniz ");
            yas = Console.ReadLine();
            Console.WriteLine("Şehrinizi Giriniz ");
            şehir = Console.ReadLine();

            Console.WriteLine("Ateşiniz var mı? ");
            ates = Console.ReadLine();//Klavyeden girilen değeri ates değişkenine atar.

            if (ates == "var")
            {
                Console.WriteLine("Nefes Darlığınız Var Mı? ");
                nefesdarlıgı = Console.ReadLine();

                if (nefesdarlıgı == "var")
                {
                    Console.ForegroundColor = ConsoleColor.Red;
                    Console.WriteLine("**En yakın sağlık kuruluşuna gidiniz**");
                }

                else


                {
                    Console.WriteLine("Öksürüğünüz Var mı");
                    öksürük = Console.ReadLine();

                    if (öksürük == "var")
                    {
                        Console.ForegroundColor = ConsoleColor.Red;
                        Console.WriteLine("**En yakın sağlık kuruluşuna gidiniz**");
                    }

                    if (öksürük == "yok")
                    {
                        Console.ForegroundColor = ConsoleColor.Red;
                        Console.WriteLine("**Diğer belirtileri gösterirseniz en yakın sağlık kuruluşuna gidiniz**");
                    }


                }


            }
            else
            {
                Console.WriteLine("Nefes darlığınız var mı?  ");
                nefesdarlıgı = Console.ReadLine();

                if (nefesdarlıgı == "var")
                {
                    Console.WriteLine("Öksürüğünüz var mı? ");
                    öksürük = Console.ReadLine();

                    if (öksürük == "var")
                    {
                        Console.ForegroundColor = ConsoleColor.Red;
                        Console.WriteLine("En yakın sağlık kuruluşuna gidiniz..");
                    }
                    else
                    {
                        Console.ForegroundColor = ConsoleColor.Red;
                        Console.WriteLine("**Diğer belirtileri gösteriyorssanız en yakın sağlık kuruluşuna gidiniz**");
                    }


                }
                else
                {
                    Console.WriteLine("öksürüğünüz var mı");
                    öksürük = Console.ReadLine();//Klavyeden girilen değeri öksürük değişkenine atar.

                    if (öksürük == "var")
                    {
                        Console.ForegroundColor = ConsoleColor.Yellow;
                        Console.WriteLine("Grip Olabilirsiniz");//Ekrana yazı yazdırma metodu.
                    }
                    else
                    {
                        Console.ForegroundColor = ConsoleColor.Green;
                        Console.WriteLine("**Evde kal**");
                    }



                }

            }
            Console.ReadKey(); //Bir tuşa basılana kadar bekler.
        }
    }
}
