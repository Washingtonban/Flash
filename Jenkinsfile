pipeline{
    agent {
        docker{
            image "justb4/jmeter"
        }
    }
    stages{
        stage("Build"){
            steps{
                sh "jmeter -v"
            }
        }
        stage("Testes"){
            steps{
                sh "jmeter -v"
            }
        }
    }
}