pipeline {
    agent any

    stages {
        stage('Validate') {
            steps {
                echo 'Building..'
		sh '/usr/share/maven/bin/mvn validate'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
		sh '/usr/share/maven/bin/mvn package'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing....'
		sh '/usr/share/maven/bin/mvn test'
            }
        }
    }
}
