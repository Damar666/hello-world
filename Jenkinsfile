pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                // Hapus baris 'cleanWs()' jika ada
                echo "Kode sudah diambil dari repositori!"
            }
        }
        stage('Final Deployment') {
            steps {
                echo "Penyalinan untuk bukti visual..."
                sh 'mkdir -p C:/JenkinsDeployTarget' 
                sh 'cp -R * C:/JenkinsDeployTarget/' 
            }
        }
    }
    // PENTING: TAMBAHKAN Bagian Pasca-Build INI
    post {
        failure {
            // Hapus folder kerja jika terjadi kegagalan
            deleteDir()
        }
        success {
            // JANGAN lakukan apa-apa, biarkan workspace tetap ada
            echo 'Workspace dipertahankan.'
        }
    }
}
