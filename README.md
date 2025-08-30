<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Salesforce Agent Test11</title>
</head>
<body>
    <h1>Salesforce Messaging Agent Test11</h1>
    <p>The chat button should appear in the bottom-right corner.</p>

    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DgK000004EU3y',
				'Messaging_For_All_Sites',
				'https://orgfarm-668524c287-dev-ed.develop.my.site.com/ESWMessagingForAllSite1756489194564',
				{
					scrt2URL: 'https://orgfarm-668524c287-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://orgfarm-668524c287-dev-ed.develop.my.site.com/ESWMessagingForAllSite1756489194564/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>



    <!-- END Salesforce Messaging Deployment Script -->

</body>
</html>
