pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                bat 'dir'
                bat 'cd venv/Scripts/ && activate && cd .. && cd .. &&  cd Portofolio &&  python manage.py test tests.tests && python manage.py test tests.form_test && python manage.py test tests.registrationtest'
                bat 'dir'
                
      
            }
        }
    }
    post {
        always {
             emailext body: 'A Test EMail', recipientProviders: ["vorobiov.daniel@gmail.com", "balaurdorina@gmail.com"], subject: 'Test'
               
                
                
        }
    }
}

