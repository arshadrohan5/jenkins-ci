node {
    checkout scm //Getting content of this repo
    stage('*** Compilation Phase ***') { // for display purposes
        //Compiling helloworld.c using bash commands
        sh '''#!/bin/bash
            gcc -g ./helloworld.c -o helloworld.out
            riscv64-unknown-elf-gcc ./helloworld.c -o helloworld_riscv_compiled.out
            riscv
         '''
    }
    stage (' *** Running Binaries ***'){
        sh '''#!/bin/bash
            ./helloworld.out
            spike /home/ali/RISCV_TOOLCHAIN_SIMULATORS/spike/riscv-pk/build/pk helloworld_riscv_compiled.out
         '''
    }
}
