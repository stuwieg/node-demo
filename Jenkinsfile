pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
// pipeline {
//   agent {
//     docker {
//       image 'node:latest'
//     }
//   }
//   stages {
//     stage('test') {
//       steps {
//         deleteDir()
//         checkout scm
//         sh 'npm install'
//         sh 'npm run lighthouse'
//       }
//       post {
//         always {
//           publishHTML(target: [
//             allowMissing: false,
//             alwaysLinkToLastBuild: false,
//             keepAll: true,
//             reportDir: '.',
//             reportFiles: 'lighthouse-report.html',
//             reportName: "Lighthouse"
//           ])
//         }
//       }
//     }
//   }
// }