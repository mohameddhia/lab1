pipeline
{
    agent any
        stages{
            stage('Pull'){
                steps{
                    script{
                        checkout([$class: 'GitSCM',branches: [[name: '*/master']] ],
                            userRemoteConfigs: [[
                                credientialsId: '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',
                                url: 'https://github.com/mohameddhia/lab1.git'
                            ]])
                    }
                }
            }
        }
}