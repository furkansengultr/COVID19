string isim, soyad, yas, şehir, ates, nefesdarlıgı, öksürük;
            Console.WriteLine("*COVID19 TANI PROGRAMI ***");

            Console.WriteLine("İsminizi Giriniz ");
            isim = Console.ReadLine();
            Console.WriteLine("Soyadınızı Giriniz ");
            soyad = Console.ReadLine();
            Console.WriteLine("Yaşınızı Giriniz ");
            yas = Console.ReadLine();
            Console.WriteLine("Şehrinizi Giriniz ");
            şehir = Console.ReadLine();

            Console.WriteLine("Ateşiniz var mı? ");
            ates = Console.ReadLine();
            if (ates == "var")
            {
                Console.WriteLine("Nefes Darlığınız Var Mı? ");
                nefesdarlıgı = Console.ReadLine();
                if (nefesdarlıgı == "var")
                {
                    Console.WriteLine("En yakın sağlık kuruluşuna gidiniz...");
                }

                else


                {
                    Console.WriteLine("Öksürüğünüz Var mı");
                    öksürük = Console.ReadLine();
                    if (öksürük == "var")
                    {
                        Console.WriteLine("En yakın sağlık kuruluşuna gidiniz..");
                    }
                    if (öksürük == "yok")
                    {
                        Console.WriteLine("Diğer belirtileri gösterirseniz en yakın sağlık kuruluşuna gidiniz..");
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
                        Console.WriteLine("En yakın sağlık kuruluşuna gidiniz..");
                    }
                    else
                    {
                        Console.WriteLine("diğer belirtileri gösteriyorssanız en yakın sağlık kuruluşuna gidiniz..");
                    }


                }
                else
                {
                    Console.WriteLine("öksürüğünüz var mı");
                    öksürük = Console.ReadLine();
                    if (öksürük == "var")
                    {
                        Console.WriteLine("Grip Olabilirsiniz");
                    }
                    else
                    {
                        Console.WriteLine("Evde kal");
                    }
                    


                }

            }
            Console.ReadKey();
