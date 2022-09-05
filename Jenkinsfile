node {
    checkout scm //Getting content of this repo
    stage('*** Compilation Phase ***') { // for display purposes
        //Compiling helloworld.c using bash commands
        sh '''#!/bin/bash
            gcc -g ./helloworld.c -o helloworld.out
         '''
    }
    stage (' *** Running Binaries ***'){
        sh '''#!/bin/bash
            ./helloworld.out
         '''
    }
}
