pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'pwd'
            }
        }
        stage('Test'){
            steps {
                sh 'ls'
            }
        }
        stage('Test world'){
            steps {
                sh 'uname -a'
            }
        }
    }
}


// stage('Build') {
//     node {
//         sh 'uname -a'
//         sh './configure --enable-debug --enable-cassert --enable-tap-tests --enable-depend'
//         sh 'make -j4'
//     }
// }

// stage('Test') {
//     parallel osx: {

//         stage('Build') {
//             node('master') {
//                 checkout scm
//                 sh 'uname -a'
//                 sh 'ls -l'
//                 sh './configure --enable-debug --enable-cassert --enable-tap-tests --enable-depend'
//                 sh 'make -j4'
//             }
//         }

//         stage('A') {
//             node('master') {
//                 sh 'make check'
//             }
//         }

//     },
//     freebsd: {
//         stage('Build') {
//             node('justscale') {
//                 checkout scm
//                 sh 'uname -a'
//                 sh 'ls -l'
//                 sh './configure --enable-debug --enable-cassert --enable-tap-tests --enable-depend'
//                 sh 'make -j4'
//             }
//         }

//         stage('A') {
//             node('justscale') {
//                 sh 'gmake check'
//             }
//         }
//     }
// }