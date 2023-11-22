@Library('my-shared-library') _

pipeline {
    agent any

    parameters {
        string(name: 'NAME', description: 'Your Name', defaultValue: 'World')
    }

    stages {
        stage('Say Hello') {
            steps {
                script {
                    HelloWorld.sayHello(params.NAME)
                }
            }
        }
    }
}
