# Azure Active Directory B2C - RealMe Assertion service - ITE Integration

** This page needs review **

This wiki explains how to integrate Real Me Assertion service in the RealMe ITE environment:

## Certificates ordering

Purchase two certificates:
1. The first one will be used to sign the SAML requests.
2. The second one will be used to integrate with the RCMS service (client certificate authentication).

## Configuring the AAD B2C tenant

You will need to generate the metadata file before completing the ITE request.

Follow the integration steps as describe for the MTS environment, but you will have to use your own cert rather than using the certificate provided by RealMe (`mts_saml_sp.p12/pfx`).

## ITE Request

1. Create a new ITE request on the [RealMe developers website](https://developers.realme.govt.nz/):
2. In ITE request, specify:
- `RCMS token required` in the **Opaque token** dropdown.
  **Needs updating - no option available here yet**
- `Return JSON identity and/or address` in the **Additional setup description** textarea.
  **Needs updating - no option available here yet**

## Obtaining the Federate Login Token

TODO Add Wiki

## Decoding identity and address claims

As part of the user journey, you can decode the safe base64 identity following this tutorial: [Decoding RealMe Claims](./Decoding-RealMe-Claims.md)

