# Tan-mlama-Eri-im-ve-D-ng-lerle-Kullan-m-
// Tanımlama  , Erişim  ve Döngülerler Dizi Kullanımı
            // Dizi Tanımlama
            string[] renkler = new string[5];// [5] dizimin boyutunu belirledim.
            string[] hayvanlar = { "KEDİ", "KÖPEK", "KUŞ" };// HAYVANLAR İSİMLİ BİR DİZİ TANIMLADIM VE ELEMANLARINI GİRDİM.
            int[] dizi;
            dizi= new int[5];   //Böylede tanımlayabiliriz.
            // Dizilere değer atama ve erişim
            renkler[0] = "Mavi";
            Console.WriteLine(hayvanlar[0]);
            dizi[3] = 10;
            Console.WriteLine(dizi[3]);
            Console.WriteLine(renkler[0]);
            Console.ReadLine();// Ekrana yazdırıyoruz.
            // Döngülerle dizi kullanımı
            // Klavyeden girilen n tane sayının ortalamasını hesaplayan program.
            Console.WriteLine("Lütfen dizinin elaman sayısını giriniz:");
            int diziUzunlugu=int.Parse(Console.ReadLine());
            int[] sayiDizisi = new int[diziUzunlugu];
            for        (int i = 0; i < diziUzunlugu; i++)
                {
                Console.WriteLine("Lütfen {0}. sayıyı giriniz.",i+1);
                sayiDizisi[i] = int.Parse(Console.ReadLine());

                    
            }
            int toplam = 0;
            foreach (var sayi in sayiDizisi)
            {
                toplam += sayi;
            }
            Console.WriteLine("Ortalama:" + toplam / diziUzunlugu);

            
        }
