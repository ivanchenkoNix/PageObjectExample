pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }

        stage('Smoke tests') {
                    steps {
                        bat 'mvn test -Dgroups=smoke'
                    }
                }
    }
}