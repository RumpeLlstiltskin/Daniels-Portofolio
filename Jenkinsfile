pipeline {
    agent { label 'master' }
    stages {
        stage('build') {
            steps {
                bat 'dir'
                bat 'cd Portofolio && dir'
                bat 'dir'
                
        //        bat ' source venv/Scripts/activate && pip install --upgrade -r requirements.txt'
            }
        }
    }
}

