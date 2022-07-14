pipeline {

    parameters {
     string(defaultValue: 'letsgo', name: 'test', trim: true)
    }
    
    agent any

    stages {
        stage('Hello') {
            steps {
                println("${params.test}")
            }
        } 
    } 

    post {
        always {
            println('Goodbye, cruel world!!')
        }
    }
}
