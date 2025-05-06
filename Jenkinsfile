pipeline {
    agent any

    stages {
        stage('Deploy se for tag') {
            when {
                branch 'refs/tags/*'
            }
            steps {
                echo "Deploy de tag"
                sh 'echo Deploy da tag...'
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