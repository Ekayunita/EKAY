import java.util.Scanner;

public class Penjualan
{
        public static void main (String[] args){

        Scanner input = new Scanner(System.in);
        //variable

         int jumlah, harga, total1, totalBayar, uang, kembalian, Sepatu, Tas, Topi, Jaket, Sendal, Baju, Jamtangan, jeans, disc = 0;
        String nama,nBarang, kelas, payments;
        String ukuran;
        
        System.out.print("=========================< Tugas Pemrograman 2 >======================\n");
        System.out.print("\t  Program Pembelian Barang Univ.Indraprasta PGRI\n");
        System.out.print("=============================< Kelompok 2 >=========================\n");
        System.out.println("");
        //daftar harga
        Baju = 45000;
        Jaket = 75000;
        Sendal = 15000;
        Sepatu = 350000;
        Topi = 20000;
        Tas = 150000;
        Jamtangan = 50000;
        jeans = 150000;
        System.out.print("\t-------------------< List Barang >-----------------\n\n");
        System.out.print("\t\tBelanja Sekarang dan Dapatkan DISKONNYA!!\n");
        System.out.print("|-----------------------------------------------------------------------|\n");
        System.out.print("|\t"+"Barang\t\t"+"|\t"+"Harga Barang\t"+"|\t"+"Ukuran\t\t|\n");
        System.out.print("|-----------------------|-----------------------"+"|-----------------------|\n");
        System.out.print("|\t"+"Baju\t"+"\t|\t"+"Rp."+Baju+"\t|\t"+"ALL SIZE\t|\n");
        System.out.print("|\t"+"Jaket\t"+"\t|\t"+"Rp."+Jaket+"\t|\t"+"ALL SIZE\t|\n");
        System.out.print("|\t"+"Sendal\t"+"\t|\t"+"Rp."+Sendal+"\t|\t"+" 38-40\t\t|\n");
        System.out.print("|\t"+"Sepatu\t"+"\t|\t"+"Rp."+Sepatu+"\t|\t"+" 38-40\t\t|\n");
        System.out.print("|\t"+"Topi\t"+"\t|\t"+"Rp."+Topi+"\t|\t"+"ALL SIZE\t|\n");
        System.out.print("|\t"+"Tas\t"+"\t|\t"+"Rp."+Tas+"\t|"+"\t  -\t\t|\n");
        System.out.print("|\t"+"Jeans\t"+"\t|\t"+"Rp."+jeans+"\t|\t"+" 30-32\t\t|\n");
        System.out.print("|\t"+"Jam Tangan"+"\t|\t"+"Rp."+Jamtangan+"\t|"+"\t  -\t\t|\n");
        System.out.print("|-----------------------------------------------------------------------"+"|\n");
        System.out.print("\n----------------------< Masukan Data >------------------------\n\n");
        System.out.print("\tMasukan Nama\t\t       "+"\t: ");
        nama = input.nextLine();
        System.out.print("\tMasukan Kelas\t\t       "+"\t: ");
        kelas = input.nextLine();
        System.out.print("--------------------------------------------------\n");
        System.out.print("\tMasukan Nama Barang    "+"\t\t: ");
        nBarang = input.nextLine();
        System.out.print("\tUkuran                 "+"\t\t: ");
        ukuran = input.next();
        System.out.print("\tHarga Barang\t  "+"\t\t: ");
        harga = input.nextInt();
        System.out.print("\tMasukan Jumlah Barang  "+"\t\t: ");
        jumlah = input.nextInt(); 
        System.out.print("\tMasukan Nominal Uang   "+"\t\t: ");
        uang = input.nextInt();
        System.out.print("\tMetode Pembayaran\t       "+"\t: ");
        payments = input.next();
        System.out.print("\n--------------------------------------------------\n");
        System.out.print("+++++++++++++++++< Nota Pembelian >+++++++++++++++\n\n");
        //Perhitungan
        total1 = jumlah * harga;
        disc = total1 * 10/100;
        totalBayar = total1 - disc;
        kembalian = uang - totalBayar;
        
        System.out.print("\tNama Pembeli\t\t\t                : "+nama+"\n");
        System.out.print("\tNama Barang\t\t\t                : "+nBarang+"\n");
        System.out.print("\tJumlah\t\t\t\t                : "+jumlah+"\n");
        System.out.print("\tUkuran\t\t\t\t                : "+ukuran+"\n");
        System.out.print("\tHarga\t\t\t\t                : "+harga+"\n");
        System.out.print("\tDiskon\t\t\t\t                : "+disc+"\n");
        System.out.print("\tMetode Pembayaran\t        : "+payments+"\n");
        System.out.print("\tTotal Bayar Sebelum Diskon\t: "+total1+"\n");
        System.out.print("\tTotal Bayar Sesudah Diskon\t: "+totalBayar+"\n");
        System.out.print("\tNominal Uang\t\t                : "+uang+"\n");
        System.out.print("\tUang Kembalian\t\t                : "+kembalian+"\n");
        System.out.print("\n+++++++++++++++++++< Terimakasih!!Selamat Datang Kembali >_< >++++++++++++++++\n");
        System.out.print("==================================================================================");
        
        
    }
}
