<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Salesforce Agent Test</title>
    <style>
        body {
            margin: 0;
            font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #f3f4f6, #e0e7ff);
            color: #333;
        }

        header {
            background: #2563eb;
            color: #fff;
            padding: 1rem 2rem;
            text-align: center;
            font-size: 1.5rem;
            font-weight: 600;
        }

        main {
            max-width: 900px;
            margin: 2rem auto;
            padding: 2rem;
            background: #fff;
            border-radius: 12px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            text-align: center;
        }

        main h1 {
            font-size: 2rem;
            color: #1e40af;
            margin-bottom: 1rem;
        }

        main p {
            font-size: 1.1rem;
            line-height: 1.6;
            margin-bottom: 2rem;
        }

        footer {
            background: #f1f5f9;
            text-align: center;
            padding: 1rem;
            font-size: 0.9rem;
            color: #555;
        }
    </style>
</head>
<body>
    <header>
        Salesforce Agent Test
    </header>

    <main>
        <h1>Welcome to Our Support Page</h1>
        <p>
            Our virtual agent is here to help you with your queries.  
            Before starting, please review our 
            <a href="https://www.salesforce.com/company/legal/" target="_blank">
                Terms & Conditions
            </a>.
        </p>
        <p>
            Once you accept, our support agent will be available in the chat window below.
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
        &copy; 2025 Salesforce Agent Test. All rights reserved.
    </footer>
</body>
</html>
