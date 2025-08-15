<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Salesforce Agent Test</title>
</head>
<body>
    <h1>Salesforce Messaging Agent Test</h1>
    <p>The chat button should appear in the bottom-right corner.</p>

    <!-- START Salesforce Messaging Deployment Script -->
    <script type='text/javascript'>
        window.addEventListener("load", function () {
            embedded_svc.settings.displayHelpButton = true; // Show the chat/help button
            embedded_svc.settings.language = 'en'; // Language setting

            embedded_svc.init(
                'https://YOUR_INSTANCE.my.salesforce.com', // Salesforce Org URL
                'https://YOUR_EXPERIENCE_SITE.force.com', // Experience Cloud site URL where messaging is deployed
                gslbBaseURL = null,
                'YOUR_DEPLOYMENT_NAME', // Deployment Name from Messaging setup
                {
                    baseLiveAgentContentURL: 'https://YOUR_INSTANCE.salesforceliveagent.com/content',
                    deploymentId: 'YOUR_DEPLOYMENT_ID', // Deployment ID from Messaging setup
                    buttonId: 'YOUR_BUTTON_ID', // Button ID from Messaging setup
                    baseLiveAgentURL: 'https://YOUR_INSTANCE.salesforceliveagent.com/chat',
                    eswLiveAgentDevName: 'YOUR_LIVE_AGENT_DEV_NAME', // Developer name from setup
                    isOfflineSupportEnabled: false
                }
            );
        });
    </script>
    <script type='text/javascript' src='https://YOUR_INSTANCE.my.salesforce.com/embeddedservice/asyncclient/bootstrap.js'></script>
    <!-- END Salesforce Messaging Deployment Script -->

</body>
</html>
