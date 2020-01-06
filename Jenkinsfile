pipeline{
    agent {
        docker{
            image "justb4/jmeter"
        }
    }
    stages{
        stage("Build"){
            steps{
                sh "chmod +x build/alpine.sh"
                sh "./build/alpine.sh"
                sh ""
            }
        }
        stage("Testes"){
            steps{
                sh "jmeter -v"
            }
        }
    }
}