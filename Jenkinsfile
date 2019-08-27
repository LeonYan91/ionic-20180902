pipeline {
    agent { docker { image 'node:10.16.3' } }
    stages {
        stage('build') {
            steps {
                sh 'npm install'
                sh 'node_modules/.bin/cordova platform add android'
                sh 'npm run build:android'
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
