pipeline{
    agent any

    tools {
        // 下面这行可以自动安装maven
       //  maven 'mvn-3.5.4'
    }

    stages {
        stage('Build'){
            steps{
                sh "mvn clean package spring-boot:repackage"
                sh "printenv" // 将环境变量打印到 console 中
            }
        }
    }
}