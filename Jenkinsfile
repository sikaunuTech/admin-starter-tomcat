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
            maven('verify')
        maven('clean verify', 'module-a/pom.xml')// withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe reports and FindBugs reports
        }
        }
    }
}