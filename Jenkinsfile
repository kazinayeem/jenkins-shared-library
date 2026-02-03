@Library('myLib') _

pipeline {
    agent { label "new-agent" }

    stages {

        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Run Docker') {
            steps {
                dockerBuild()
            }
        }
    }
}
