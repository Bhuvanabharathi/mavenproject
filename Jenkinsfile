pipeline {

    agent any

    stages{

        stage('clone the code') {

            steps {

                git 'https://github.com/himanshurathi/mavenproject'

                sh 'mvn clean package'

            }

       }
	stage('Approval'){
steps{
	input('do you want to deploy it?')
}
}
stage('Deploy'){
steps{
sh 'mvn install'
}
}

    }

}

