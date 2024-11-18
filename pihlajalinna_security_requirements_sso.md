15.02.2024

Azure SSO
- Implementation not that much
  - Identity service in between our system and Azure that manages the authentication (eg. AWS Cognito)
  - Our system verifies the reuqests coming from AWS Cognito
  - Add feature to UI to select SSO --> forward to AWS Conginot --> forward back to DMS to fetch the token from AWS
  - relay authetization request - receive authentication code - retreive the token for OICD
    -> Get information about the user
  - Admin creates users in the DMS.
  - Login first with email as password to log in and click to connect to Auzre AD. Emails are different in Azure AD so we tie it.

What is required from them?
  - Can we have an account in their Azure AD from the to test?
  - 

- but requires a security audit
- Default UI for selection from a list of available oranization (Pihlajalinna, Terveystalo)
  - Alternative is to fill in email --> and then reveal the list
  - A direct link

Lokien toimittaminen Pihlajalinnan SOC -palveluun ja IP -rajaus kirjautumiselle


# Questions
- Pihlajalinna -> multiple organizations with SSO
- IDP logs only the authetication requests: no information if login to DMS was successful.
- When deleting an account do they need some information about the action? They can go check from the DMS user managemet. Is this enough?