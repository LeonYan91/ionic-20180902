pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'npm install'

//                 sh 'echo $ANDROID_HOME'
                    sh 'hostname'
                    sh 'hostname -i'
//                    sh 'ls /usr -a'
                    sh 'java -v'
                    sh 'echo $GRADLE_HOME'

                    sh 'gradle -v'


//                 sh 'java -version'
                sh 'node_modules/.bin/cordova build android'
//                 sh 'echo $ANDROID_HOME'
//                 sh 'npm run build:android'
            }
        }

//         stage('deploy') {
//                     steps {
//                         sh 'echo start deploying#####'
//
//                         sshPublisher(publishers: [sshPublisherDesc(configName: 'trainingserver', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/opt/expressapp/express-20190822/public/', remoteDirectorySDF: false, removePrefix: 'build', sourceFiles: 'build/**')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
//
//                     }
//
//
//                 }
    }
}
