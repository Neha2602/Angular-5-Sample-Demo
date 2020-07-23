node {
         stage ('Checkout SCM'){
                    git branch: 'master',url: 'https://github.com/Neha2602/Angular-5-Sample-Demo.git'
         }
         
         stage('Install node modules'){
                      bat "npm install"
         }
         stage('Build'){
                     bat "npm install @angular-devkit/core"
                     bat "npm run ng build"           
         }
         stage('Deploy'){
                      bat "pm2 restart all"
         }
     }
