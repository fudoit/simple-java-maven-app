pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /Users/fufu/jks/.m2:/root/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh   'mvn -B -DskipTests clean package' 
		echo 'helo wd'
            }
        }
    }
}
