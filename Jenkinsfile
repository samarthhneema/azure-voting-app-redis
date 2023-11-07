pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            echo "$GIT_BRANCH"
         }
      }
      stage('Docker Build') {
         steps 
            sh(script: 'docker compose build')
            // powershell(script: 'docker images -a')
            //Single line script or single call in ''
            // powershell(script: """
            //      cd azure-vote/
            //      docker images -a
            //      docker build -t jenkins-pipeline .
            //      docker images -a
            //      cd ..
            //      """ )
                 //Where as to run multiple commands we do """...."""
                 //Docker powershell script 
         
      }
   //    stage('Start App') {
   //       steps {
   //          sh(script: 'docker compose up -d')
   //       }
   //    }
   //    stage('Run Tests') {
   //       steps {
   //          sh(script: """
  
   //          pip3 install numpy pytest
   //          python -m pytest ./tests/test_sample.py
            
            
            
   //          """)
   //       }
   //       post {
   //          success {
   //             echo "Tests passed! :)"
   //          }
   //          failure {
   //             echo "Tests failed :("
   //          }
   //       }
   //    }
   // }
   // post {
   //    always {
   //       sh(script: 'docker compose down')
   //    }
   }
}