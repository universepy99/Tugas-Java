# Tugas-Java
andika rizki harahap tugas java kelas ti 22 j
public class GajiKaryawan {
    public static void main(String[] args) {
        String nama = "Andika Rizki Harahap";
        int golonganGaji = 3;
        int jumlahAnak = 1;
        int lembur = 4;

        // Menghitung gaji pokok
        int gajiPokok = 0;
        if (golonganGaji == 1) {
            gajiPokok = 1500000;
        } else if (golonganGaji == 2) {
            gajiPokok = 2500000;
        } else if (golonganGaji == 3) {
            gajiPokok = 3500000;
        }

        // Menghitung tunjangan anak
        int tunjanganAnak = 0;
        if (jumlahAnak > 2) {
            tunjanganAnak = 1000000;
        } else if (jumlahAnak >= 1 && jumlahAnak <= 2) {
            tunjanganAnak = 500000;
        }

        // Menghitung gaji lembur
        int gajiLembur = lembur * 200000;

        // Menghitung total gaji
        int totalGaji = gajiPokok + tunjanganAnak + gajiLembur;

        System.out.println("Nama: " + nama);
        System.out.println("Golongan gaji: " + golonganGaji);
        System.out.println("Jumlah anak: " + jumlahAnak);
        System.out.println("Lembur: " + lembur + " hari");
        System.out.println("Gaji pokok: " + gajiPokok);
        System.out.println("Tunjangan anak: " + tunjanganAnak);
        System.out.println("Gaji lembur: " + gajiLembur);
        System.out.println("Total gaji: " + totalGaji);
    }
}
