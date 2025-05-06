pipeline {
    agent any

    stages {
        stage('Deploy se for tag') {
            when {
                buildingTag()
            }
            steps {
                echo "Ação super ultra mega hyper turbo blaster."
                sh 'echo Deploy de release...'
            }
        }
    }

    post {
        success {
            echo "Pipeline finalizado com SUCESSO"
        }
        failure {
            echo "Pipeline FALHOU."
        }
    }
}