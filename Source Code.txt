/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package diskon_pembelian;
import java.util.Scanner;
//        Rass
//        Rass
//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass
//        Rass //        Rass
//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass
//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass//        Rass
//        Rass//        Rass//        Rass//        Rass//        Rass



public class Diskon_Pembelian {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Scanner sc = new Scanner (System.in);
//        Rass
//Variabelnya
        int harga;
        int jumlah;
        int diskon;
        int total;
        float pembayaran;
        String nama;
        
        
        
        System.out.println("Inputkan Nama Anda           : ");
        nama = sc.next();
        
        System.out.println("\n------------Selamat Datang di Program Saya AlFiras Manar_A082_009------------");
        
        System.out.println("\nMasukan harga barang disini  :");
        harga = sc.nextInt();
        System.out.println("Masukan jumlah barang        :");
        jumlah = sc.nextInt();
                                
        total= jumlah * harga;
                                        
        if(total <= 100001){//        Rass
            diskon = total;//     //        Rass
            total = total;//        Rass
            System.out.println("Tidak Ada Diskon : 0%");
            System.out.println("Total Belanjaan  : " + harga);
            
        } else if (total >= 100001 && total <= 200000){
            diskon = total * 5/100;//        Rass
            total = total - diskon;//        Rass
            System.out.println("Diskon Ada       : 5%");//        Rass
            System.out.println("Total Belanjaan  : " + total);//        Rass
            
        } else if (total >= 200001 && total <= 300000) {
            diskon = total * 10/100; //        Rass
            total = total - diskon;//        Rass
            System.out.println("Diskon Ada       : 10%");
            System.out.println("Total Belanjaan  : " + total);
        } else if (total >= 300001 && total <= 400000) {
            diskon = total * 15/100;//        Rass
            total = total - diskon;//        Rass
            System.out.println("Diskon Ada       : 15%");
            System.out.println("Total Belanjaan  : " + total);
        } else if (total >=400001 && total <= 500000) {
            diskon = total * 20/100;//        Rass
            total = total - diskon;//        Rass
            System.out.println("Diskon Ada       : 20%");
            System.out.println("Total Belanjaan  : " + total);
        } else if (total >= 500001) {//        Rass
            diskon = total * 25/100;//        Rass
            total = total - diskon;//        Rass
            System.out.println("Diskon Ada       : 25%");
            System.out.println("Total Belanjaan  : " + total);
        }//        Rass
        
        System.out.println("----------Pembayaran----------");
        //        Rass
        System.out.println("\nHalo Bapak/Ibu                         :" + nama);
        System.out.println("Tagihan Anda                            : " + total);
        //        Rass
        System.out.print("\nMasukan Nominal Uang                  Rp: ");
            pembayaran = sc.nextFloat();
            //        Rass
            double kembalian = pembayaran - total;
            //        Rass
             if(pembayaran >= total){
                System.out.println("Kembalian Anda                 Rp: " + kembalian);
                System.out.println("\nTransaksi Sukses Happy Shoping :)");
                //        Rass
            } else if(pembayaran < total) {
                System.out.println("----------------------");
                System.out.println("Uang Anda Kurengg Bos!!!");
                System.out.println("----------------------");
                System.out.print("Masukan Nominal Uang              Rp: ");
                pembayaran = sc.nextFloat();
                //        Rass
                System.out.println("Kembalian Anda                  Rp: " + kembalian);
                System.out.println("\nTransaksi Sukses Happy Shoping :)");
            }
    }
    
}
