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
                /*
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                    */
                    echo M2_HOME="${M2_HOME:-/usr/share/maven}"
                    echo JAVA_HOME= "${M2_HOME/bin/mvn}" "$@"
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
