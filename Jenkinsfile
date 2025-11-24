pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                echo "Kode sudah diambil dari repositori!"
            }
        }
        stage('Verifikasi Workspace') { // Stage Baru untuk Membuktikan File Ada
            steps {
                echo "Memverifikasi isi workspace..."
                sh 'ls -l' // Perintah untuk menampilkan daftar file (seperti di screenshot Anda)
                echo "Verifikasi selesai."
            }
        }
        stage('Deployment') {
            steps {
                echo "Deployment Otomatis Berjalan..."
                // Tambahkan perintah deploy sesungguhnya di sini
            }
        }
    }
}
