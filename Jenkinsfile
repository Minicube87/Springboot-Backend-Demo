pipeline{

    agent label any


    tools{
        maven 'Maven'
    }

    stages{
        stage("Cleanup"){
            steps{
              sh "mvn --version"  
              sh "mvn clean"
            }
        }
    }
    post{
        always{
          echo "dsadsadas"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}