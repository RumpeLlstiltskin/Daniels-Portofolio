pipeline{
    agent any
    options {
        timestamps()
    }
    stages {
        stage('build'){
            steps{
                script{
                cd Portofolio
                python manage.py test Portofolio.tests   
                }
            }
        }
    }
}
