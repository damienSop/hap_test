pipeline {
  agent any
  stages {
    stage('User Input') {
        steps {
            script {
                // Define the options for the select input
                def options = ['Option 1', 'Option 2', 'Option 3']

                // Prompt the user for input and store the selected option in a variable
                def userInput = input(
                    id: 'selectInput',
                    message: 'Please select an option:',
                    parameters: [
                        choice(choices: options, description: 'Select an option')
                    ]
                )

                // Use the selected option in your pipeline logic
                echo "Selected option: ${userInput}"
                }
            }
        }
    }
}