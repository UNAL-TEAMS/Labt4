#!groovy

node {

    try {

       stage 'Checkout'
            checkout scm

       stage 'Test'

            env.NODE_ENV = "test"

            print "Environment will be : ${env.NODE_ENV}"

            sh 'node -v'
            sh 'npm prune'
            sh 'npm install'
            sh 'npm test'

       stage 'Deploy'
            print "Nah, nothing is really deployed, just testing..."
    }
    catch (err) {

        throw err
    }

}
