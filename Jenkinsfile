pipeline
{
    agent any
        stages{
            stage('Pull'){
                steps{
                    script{
                        checkout([$class: 'GitSCM',branches: [[name: '*/master']] ],
                            userRemoteConfigs: [[
                                credientialsId: 'dhia-lab1',
                                url: 'https://github.com/mohameddhia/lab1.git'
                            ]])
                    }
                }
            }
        }
}