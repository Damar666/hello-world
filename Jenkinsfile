pipeline {
    agent any // PENTING: Mendefinisikan agent di level pipeline
    stages {
        stage('Checkout') {
            steps {
                // Jenkins otomatis checkout di agent any
                echo "Kode sudah diambil dari repositori!"
            }
        }
        stage('Deployment') {
            steps {
                echo "Memulai Deployment Otomatis..."
                
                // Perintah untuk melihat file di workspace
                sh 'ls -l' 
                
                echo "Deployment Selesai."
            }
        }
    }
    // Opsi untuk memastikan workspace tetap ada
    options {
        skipDefaultCheckout true // Biasanya tidak perlu, tapi bisa membantu.
    }
}
