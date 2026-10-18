@Library("JenkinsPipelines") _ // See https://github.com/mwdle/JenkinsPipelines

boolean disableIndexTriggers = env.BRANCH_NAME != 'main'

quadletPipeline(
    disableIndexTriggers: disableIndexTriggers,
    podmanSecretMappings: [
        [
            type: 'usernamePassword',
            credentialsId: 'Email noreply',
            podmanSecretUsernameName: 'lab_smtp_username',
            podmanSecretPasswordName: 'lab_smtp_password'
        ]
    ]
)
