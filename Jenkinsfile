pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                echo "Kode sudah diambil dari repositori!"
            }
        }
        stage('Deployment') {
            steps {
                echo "Memulai Deployment ke folder target di C drive..."
                
                // Pastikan folder ini ADA di C: drive Anda
                sh 'mkdir -p C:/JenkinsDeployTarget' 
                
                // Menyalin SEMUA file dari workspace (yang tidak ditampilkan) ke folder C: drive
                sh 'cp -r * C:/JenkinsDeployTarget/' 
                
                echo "Deployment Selesai. Cek folder C:/JenkinsDeployTarget"
            }
        }
    }
}
