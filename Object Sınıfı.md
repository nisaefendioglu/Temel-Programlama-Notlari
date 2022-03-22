## OBJECT SINIFI​
Diziler içerisinde aynı tip verilerimizi barındırabileceğimiz bilgisini vermiştik. Fakat farklı tipteki verileri barındırmak için de diziler için bir sınıf mevcuttur. Bu sınıf Object sınıfı olarak geçmektedir.​

Java’da her sınıf Object sınıfından türetildiği için böyle bir istisna mevcuttur.​

Dizimizi Object sınıfı kullanarak oluşturmamız durumunda içerisinde farklı tipteki verileri de ekleyebiliriz.​

## Object Sınıfı Örnek Tanımlama​
 Object dizi [] = new Object[3] ; //3 elemanlı bir dizi oluşturduk.​

    dizi[0] = "Mehmet";​

    dizi[1] = 2;​

    dizi[2] = 5.9;​

Örnek :
Object sınıfını kullanarak 5 elemanlı bir dizi oluşturunuz ve bu dizi içerisindeki tüm elemanları ekrana yazdırınız.​

        public static void main(String[] args) {
        Object [] dizi = {"Nisa", 15, "Java Dersleri", 3, 7}; 
        for(int i=0; i<=dizi.length; i++)
        System.out.println(dizi[i]);
        }
