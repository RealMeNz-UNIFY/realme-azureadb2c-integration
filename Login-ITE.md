### Azure Active Directory B2C - RealMe Login service - ITE Integration

This wiki explains how to integrate Real Me Login in the RealMe ITE environment:

1. Purchase a certificate: it will be used to sign the SAML requests.

2. Download the [ITE login service IdP metadata zip file](https://developers.realme.govt.nz/assets/ITE-Login-service-bundle-2023.zip). It contains the ITE SAML Metadata (`B2C_1A_DIA_RealMe_LoginService.xml`)

3. Follow the integration steps as describe for the MTS environment:
- Use your own cert rather than the certificate provided by RealMe (`mts_saml_sp.pfx`).

1. Create An ITE Integration Request on the [RealMe developers website](https://developers.realme.govt.nz/)
