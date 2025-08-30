<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sathya AgentForce Webpage</title>
    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f1f5f9, #e0e7ff);
            color: #333;
        }

        header {
            background: #0f172a;
            color: #fff;
            padding: 1.5rem 2rem;
            text-align: center;
            font-size: 2rem;
            font-weight: 700;
            letter-spacing: 1px;
            box-shadow: 0 3px 6px rgba(0,0,0,0.15);
        }

        main {
            max-width: 900px;
            margin: 3rem auto;
            padding: 2.5rem;
            background: #fff;
            border-radius: 14px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.12);
            text-align: center;
        }

        main h1 {
            font-size: 2.2rem;
            color: #1d4ed8;
            margin-bottom: 1rem;
        }

        main p {
            font-size: 1.15rem;
            line-height: 1.6;
            margin-bottom: 2rem;
            color: #444;
        }

        footer {
            background: #f8fafc;
            text-align: center;
            padding: 1rem;
            font-size: 0.9rem;
            color: #555;
            border-top: 1px solid #e5e7eb;
        }
    </style>
</head>
<body>
    <header>
        Sathya AgentForce Webpage
    </header>

    <main>
        <h1>Welcome to Sathya’s AgentForce</h1>
        <p>
            This is your personalized AgentForce webpage.  
            Use the chat widget in the corner to connect with your Salesforce Agent.
        </p>
    </main>

    <!-- Salesforce Embedded Messaging Deployment Script -->
    <script type='text/javascript'>
        function initEmbeddedMessaging() {
            try {
                embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

                embeddedservice_bootstrap.init(
                    '00DgK000004EU3y',
                    'Matching_Candidates',
                    'https://orgfarm-668524c287-dev-ed.develop.my.site.com/ESWMatchingCandidates1755258613638',
                    {
                        scrt2URL: 'https://orgfarm-668524c287-dev-ed.develop.my.salesforce-scrt.com'
                    }
                );
            } catch (err) {
                console.error('Error loading Embedded Messaging: ', err);
            }
        };
    </script>
    <script type='text/javascript' src='https://orgfarm-668524c287-dev-ed.develop.my.site.com/ESWMatchingCandidates1755258613638/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
    <!-- END Salesforce Messaging Deployment Script -->

    <footer>
        &copy; 2025 Sathya AgentForce. All rights reserved.
    </footer>
</body>
</html>
