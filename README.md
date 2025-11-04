# LatihanUKLSoalSulitNo2-Jasmine-Salsabila-F.-W.-XRPL2-
Fungsi dari program ini adalah untuk mengetahui hasil dari penjumlahan 2 buah matriks. Lalu cara kerjanya adalah dengan cara menginputkan elemen matriks  oleh user.

Berikut adalah kode programnya:

    import java.util.Scanner;
    public class SoalSulitNo2 {
    
    public static void main(String[] args) {
        Scanner inputan = new Scanner(System.in);

        System.out.println("Masukkan Jumlah Baris: ");
        int baris = inputan.nextInt();
        System.out.println("Masukkan Jumlah Kolom: ");
        int kolom = inputan.nextInt();

        int[][] matriksA = new int[baris][kolom];
        int[][] matriksB = new int[baris][kolom];
        int[][] hasil = new int[baris][kolom];

        System.out.println("Masukkan Elemen Matriks A: ");
        for(int i = 0; i < baris; i++) {
            for(int j = 0; j < kolom; j++) {
                System.out.print("A["+ i +"]["+ j +"] = ");
                matriksA[i][j] = inputan.nextInt();
            }
        }

        System.out.println("Masukkan Elemen Matriks B: ");
        for(int i = 0; i < baris; i++) {
            for(int j = 0; j < kolom; j++) {
                System.out.print("B["+ i +"]["+ j +"] = ");
                matriksB[i][j] = inputan.nextInt();
            }
        }

        for(int i = 0; i < baris; i++) {
            for(int j = 0; j < kolom; j++) {
                hasil[i][j] = matriksA[i][j] + matriksB[i][j];
            }
        }

        System.out.println("HASIL PENJUMLAHAN MATRIKS A DAN B");
        for(int i = 0; i < baris; i++) {
            for(int j = 0; j < kolom; j++) {
                System.out.print(hasil[i][j] + "\t");
            }
            System.out.println();
        }

        inputan.close();
        }
    }
