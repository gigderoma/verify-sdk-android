# Changelog Android

## Verify SDK 2.0.4 (26.07.2019)
- Fix on-premises filtering of pending transactions by `authenticator_id`
- Fix NPE when OAuth token could not be decrypted
- Fix KeyStore exception `android.os.ServiceSpecificException` in Android P
- Update lower boundary for TOTP period to 1 (second)
- Update targeted Android API to 29
- Enhances TOTP enrolment parsing for on-premises authenticators

## Verify SDK 2.0.3 (04.04.2019)
- Update on-premise transaction signing data value for ISAM v9.0.6.
- Support QR code login for Cloud and On-Premise.
- Support `DEVICE_ROOTED` detection.
- Enhance transaction data parsing of additional data to support custom JSON attributes.
- Expose the transaction timestamp in `PendingTransactions`.
- Prevent QR scanning where the TOTP period is less than 10 or greater than 300.
- Enforce Android API version 23 or greater for using the SDK

## Verify SDK 2.0.2 (10.10.2018)
- support certificate pinning 
- support default implementations for `ignoreSsl == true`

## Verify SDK 2.0.1
- n/a

## Verify SDK 2.0.0
- replacing Mobile Access SDK v1
- supporting both on-premises and cloud based multi-factor authenticators
- enhanced security features that apply to both on-premise and cloud


## Mobile Access SDK v1.2.6
- Support for checking if key pair exists

## Mobile Access SDK v1.2.5 (05.09.2017)
- Support parenthesis in url query part
- Support for determining if keys may be invalidated.
- Support for using authenticated keys for signing.
- Exposing error code from 'MobileKitException' class.
- Exposing algorithm and keystore name from 'KeyStoreHelper' class.

## Mobile Access SDK v1.2.4 (18.07.2017)
- Support for custom headers in OAuthContext.
- Support Base64 encoding options for public key export and data signing.
- Support for logging output to logcat
- Support for customised exception class 'MobileKitException'
- Accepts both "SHAx" and "HmacSHAx" as input for HmacAlgorithm.

## Mobile Access SDK v1.2.0 (30.09.2016)
- Support for internationalisation.
    * Czech, German, Spanish, French, Hungarian, Italian, Japanese, Korean, Polish, Portuguese, Russian, Chinese (Simplified and Taiwan)

- rename library to "IBMMobileKit-<version_number>.aar"

- Support for multi-factor (MFA) and non-MFA authentication enrolment
    * Fingerprint
    * User presence enrolment
    * HOTP enrolment
    * TOTP enrolment

- Support for multi-factor (MFA) authentication unenrollment
    * Fingerprint
    * User presence enrolment

- Support for context based challenge and verification
    * Fingerprint
    * User presence enrolment
    * HOTP enrolment
    * TOTP enrolment
    * Username password
- Support for extending the context based challenge framework
- Support for querying pending challenges

## Mobile Access SDK v1.0.0 (26.05.2016)
- Support for OAuth ROPC and AZN code flow
- Support for HMAC generated one-time password (HOTP)
- Support for time generated one-time password (TOTP)
