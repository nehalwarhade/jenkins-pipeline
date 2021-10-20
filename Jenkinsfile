pipeline {
    agent any
    tools { 
        maven 'Maven' 
        jdk 'JDK 1.8' 
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${M2_HOME}/bin:${PATH}"
                    echo "M2_HOME = /usr/share/maven"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
    }
}


/*
pipeline { 
    agent any  
    stages { 
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.' 
            }
        }
    }
}
*/
