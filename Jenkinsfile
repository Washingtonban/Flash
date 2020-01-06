pipeline{
    agent {
        docker{
            image "justb4/jmeter"
        }
    }
    stages{
        stage("Build"){
            steps{
                sh "Bump"
            }
        }
        stage("Testes"){
            steps{
                sh "jmeter -v"
            }
        }
    }
}