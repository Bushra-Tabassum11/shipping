@Library('roboshop-shared-library') _

env.REPONAME="shipping"
env.TFDIR="mutable-infra"
backendInfra()


// pipeline {
//     agent any
//     options {
//         ansiColor('xterm')
//     }
//     parameters {
//         choice(name: 'ENV', choices: ['dev', 'prod'], description: 'Select The Environment')
//         choice(name: 'ACTION', choices: ['apply', 'destroy'], description: 'Select Create or Destroy')
//     }

//     stages {
//         stage('terraform init') {
//             steps { 
//                     // When you intend to use any groovy commands or any syntax, enclose them inside scritp {}
//                     script { git branch: 'main', url: 'https://github.com/b54-clouddevops/cart.git' }
//                     sh "ls -ltr"
//                     sh "pwd"
//                     sh "cd ${WORKSPACE}/mutable-infra"   
//                     sh "ls -ltr"
//                     sh "terrafile -f env-${ENV}/Terrafile"
//                     sh "terraform init -backend-config=env-${ENV}/${ENV}-backend.tfvars"
//             }
//         }

//         stage('terraform plan') {
//             steps { 
//                     sh "cd mutable-infra" 
//                     sh "terraform plan -var-file=env-${ENV}/${ENV}.tfvars"
//             }
//         }

//         stage('terraform apply') {
//             steps { 
//                     sh "cd mutable-infra" 
//                     sh "terraform ${ACTION} -auto-approve -var-file=env-${ENV}/${ENV}.tfvars"
//             }
//         }
//     }
// }

