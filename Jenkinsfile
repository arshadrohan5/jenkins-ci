node {
    def mvnHome
    stage('Preparation') { // for display purposes
        // Get some code from a GitHub repository
        git 'https://github.com/jglick/simple-maven-project-with-tests.git'
        // Get the Maven tool.
        // ** NOTE: This 'M3' Maven tool must be configured
        // **       in the global configuration.
//         mvnHome = tool 'M3'
    }
}
// node {
//     stage(' *** Installing GCC in Jenkins ***') {
//         gcc -g ./helloworld.c
// //       echo "HELLO WORLD !\n"
//     }
// }
