pipeline {
        agent any
        stages {
            stage('Compile stage') {
                steps {
                    maven(maven : 'Maven 3.3.9'){
                        bat "mvn clean compile"
                }
            }
        }

             stage('testing stage') {
                 steps {
                    maven(maven : 'Maven 3.3.9'){
                        bat "mvn test"
                }
            }
        }

              stage('deployment stage') {
                  steps {
                    maven(maven : 'Maven 3.3.9'){
                        bat "mvn deploy"
                }
            }
        }

      }

    }
