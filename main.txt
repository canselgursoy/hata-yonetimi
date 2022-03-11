using System;
namespace hata_yonetimi
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                Console.WriteLine("Bir sayı giriniz:");
                int sayi =Convert.ToInt32(Console.ReadLine());
                Console.WriteLine("Girmiş olduğunuz sayı:"+sayi);



            }
            catch(Exception ex)
            {
                Console.WriteLine("Hata: "+ ex.Message.ToString());


            }

            try
            {
                int a= int.Parse(null);

            }
            catch (ArgumentNullException ex)
            {
             Console.WriteLine("Boş değer girdiniz");
             Console.WriteLine(ex);
             

            finally
            {
                Console.WriteLine("İşlem başarıyla tamamlandı.");
                
            }

            }
        }
    }
}
