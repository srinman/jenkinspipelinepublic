pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'ls prog1.py' 
            }
        }
        stage('Test'){
            steps {
                sh 'python prog1.py > prog1.output'
            }
        }
        stage('Deploy') {
            steps {
                sh 'python prog1.py'
            }
        }
    }
}
