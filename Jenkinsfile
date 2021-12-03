pipeline{
    agent any
    stages{
        stage('code'){
            steps{
                echo 'testing this and that'
            }
        }
        stage('Build') {
            steps{
            ls 
            withMaven {
                    sh "mvn clean verify"
            } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
        }
        }
    }
}