pipeline {
    agent any

    // Opsi untuk Pipeline, bisa dihilangkan jika tidak perlu
    options {
        skipDefaultCheckout(false) 
    }

    stages {
        stage('Checkout') {
            steps {
                // Bersihkan workspace dari build sebelumnya (opsional)
                cleanWs(deleteDirs: true) 
                
                // Melakukan checkout kode
                // (Biasanya dilakukan secara otomatis oleh Git SCM, tapi kita definisikan untuk eksplisit)
                checkout scm 
                
                echo "Kode sudah diambil dari repositori!"
            }
        }
        stage('Verifikasi') {
            steps {
                // Perintah untuk menampilkan daftar file (hanya untuk log)
                sh 'ls -l'
            }
        }
        stage('Deployment') {
            steps {
                echo "Deployment Otomatis Berjalan..."
            }
        }
    }
}
