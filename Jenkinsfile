boolean disableIndexTriggers = env.BRANCH_NAME != 'main'

quadletPipeline(
    disableIndexTriggers: disableIndexTriggers,
    podmanSecretMappings: [
        [
            type: 'usernamePassword',
            credentialsId: 'Email noreply',
            podmanSecretPasswordName: 'lab_smtp_password',
            podmanSecretUsernameName: 'lab_smtp_username'
        ]
    ]
)
