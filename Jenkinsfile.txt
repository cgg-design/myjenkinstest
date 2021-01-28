pipeline {
    agent any 
            stages {
                stage('Build') { 
                    steps {
                        echo 'Building the application'
                    }
                }
                stage('test') { 
                    steps {
                         echo 'Testing the application'
                    }
                }
                stage('deploy') { 
                            steps {
                                echo'deploying the application'
                            }

                }
                stage('Some') { 
                            steps {
                                echo'Another job '
                            }
                }
            }
}
