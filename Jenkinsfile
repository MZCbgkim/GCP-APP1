pipeline {
    agent any

    stages {
        stage('Source') {
            steps {
                script {
                    echo 'GIT'
                    sh 'sleep 2'
                }
            }
        }

        stage('parallel Build') {
            parallel {
                stage('Build 1') {
                    steps {
                        echo 'Build 1'
                        sh 'sleep 1'
                    }
                }
                stage('Build 2') {
                    steps {
                        echo 'Build 2'
                        sh 'sleep 1'
                    }
                }
                stage('Build 3') {
                    steps {
                        echo 'Build 3'
                        sh 'sleep 1'
                    }
                }
                stage('Build 4') {
                    steps {
                        echo 'Build 4'
                        sh 'sleep 1'
                    }
                }
                stage('Build 5') {
                    steps {
                        echo 'Build 5'
                        sh 'sleep 1'
                    }
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo 'Selenium'
                    sh 'sleep 3'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                script {
                    echo 'Ansible'
                    sh 'sleep 2'
                }
            }
        }
        
    }
}
