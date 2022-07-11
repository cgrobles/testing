pipeline {

    parameters {
     string(defaultValue: '_notdef_', name: 'test', trim: true)
    }
    
    agent any

    stages {
        stage('Hello') {
            steps {
                println("${params.test}")
                echo "tusmuertos"
            }
        } 
    } 

    post {
        always {
            println('Goodbye, cruel world!!')
        }
    }
}
