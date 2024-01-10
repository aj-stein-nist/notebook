file:: [rfc7517.txt_1703615336839_0.pdf](../assets/rfc7517.txt_1703615336839_0.pdf)
file-path:: ../assets/rfc7517.txt_1703615336839_0.pdf

- In addition to the common parameters, each JWK will have members that are key type specific. These members represent the parameters of the key. Section 6 of the JSON Web Algorithms (JWA) [JWA] specification defines multiple kinds of cryptographic keys and their associated members.
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b1d5e-d4e8-4a06-9040-b36fbb763c4f
- The member names within a JWK MUST be unique; JWK parsers MUST either reject JWKs with duplicate member names or use a JSON parser that returns only the lexically last duplicate member name, as specified in Section 15.12 (The JSON Object) of ECMAScript 5.1 [ECMAScript].
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b1d75-a15e-4764-bf0f-88032ad7aac5
- Additional members can be present in the JWK;
  ls-type:: annotation
  hl-page:: 5
  hl-color:: blue
  id:: 658b1d82-ef2e-46d4-925a-8debe9f0bb99
- "kty" (Key Type) Parameter
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b1da3-6f4d-4a42-b9f7-93968ca4bf02
- The "kty" value is a case-sensitive string. This member MUST be present in a JWK.
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b1db9-5995-436a-b1fb-4a6fde85a3d9
- "use" (Public Key Use) Parameter
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b1dcd-306d-498e-9de0-9637446ec7b2
- Values defined by this specification are: o "sig" (signature) o "enc" (encryption)
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b1dea-cefc-446d-9709-2bc0a6ff262f
- Other values MAY be used. The "use" value is a case-sensitive string. Use of the "use" member is OPTIONAL, unless the application requires its presence.
  ls-type:: annotation
  hl-page:: 6
  hl-color:: blue
  id:: 658b1dfd-bef4-4818-a24a-79e90822c2b0
- "key_ops" (Key Operations) Parameter
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b1e15-9bd0-4f6c-8262-f969e89e7ba5
- Its value is an array of key operation values. Values defined by this specification are: o "sign" (compute digital signature or MAC) o "verify" (verify digital signature or MAC) o "encrypt" (encrypt content) o "decrypt" (decrypt content and validate decryption, if applicable) o "wrapKey" (encrypt key) o "unwrapKey" (decrypt key and validate decryption, if applicable) o "deriveKey" (derive key) o "deriveBits" (derive bits not to be used as a key)
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b1e2d-1030-430d-8767-e40d3326be25
- Note that the "key_ops" values intentionally match the "KeyUsage" values defined in the Web Cryptography API[W3C.CR-WebCryptoAPI-20141211] specification.
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b1e3b-4bf3-4b24-b03e-29c7ce0ffa52
- Multiple unrelated key operations SHOULD NOT be specified for a key because of the potential vulnerabilities associated with using the same key with multiple algorithms.
  ls-type:: annotation
  hl-page:: 7
  hl-color:: blue
  id:: 658b1e4f-dfc8-45fb-bb8e-f25c4d48a5c8
- "alg" (Algorithm) Parameter
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1e61-073d-4731-a08a-5a5cdebc52cf
- The "alg" value is a case-sensitive ASCII string. Use of this member is OPTIONAL.
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1e7c-d612-487d-83f4-9a5afc747cd3
- "kid" (Key ID) Parameter
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1e8a-f9ae-49e9-8dcd-63eca8d75139
- This is used, for instance, to choose among a set of keys within a JWK Set during key rollover. The structure of the "kid" value is unspecified. When "kid" values are used within a JWK Set, different keys within the JWK Set SHOULD use distinct "kid" values.
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1ea6-d814-4bb8-a8a4-99e4d86af71e
- "x5u" (X.509 URL) Parameter
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1ecc-8e06-430e-9100-27266c2f89c0
- The identified resource MUST provide a representation of the certificate or certificate chain that conforms to RFC 5280[RFC5280] in PEM-encoded form, with each certificate delimited as specified in Section 6.1 of RFC 4945 [RFC4945].
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1ee1-d9ad-443d-9332-46430803d9be
- The protocol used to acquire the resource MUST provide integrity protection; an HTTP GET request to retrieve the certificate MUST use TLS [RFC2818] [RFC5246]; the identity of the server MUST be validated, as per Section 6 of RFC 6125 [RFC6125]. Use of this member is OPTIONAL.
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1eff-1582-4340-830c-18a2203e3f33
- If other members are present, the contents of those members MUST be semantically consistent with the related fields in the first certificate.
  ls-type:: annotation
  hl-page:: 8
  hl-color:: blue
  id:: 658b1f20-68a1-43c3-a0a8-55d3814e9917
- "x5c" (X.509 Certificate Chain) Parameter
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 658b1f31-0242-4032-a15b-5a4f9d6bee87
- The certificate chain is represented as a JSON array of certificate value strings. Each string in the array is a base64-encoded (Section 4 of [RFC4648] -not base64url-encoded) DER [ITU.X690.1994] PKIX certificate value. The PKIX certificate containing the key value MUST be the first certificate. This MAY be followed by additional certificates, with each subsequent certificate being the one used to certify the previous one.
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 658b1f53-aa82-4c8c-a063-495da30e0e13
- "x5t" (X.509 Certificate SHA-1 Thumbprint) Parameter
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 658b1f76-7d2a-4f06-89b3-72b28778091e
- The "x5t" (X.509 certificate SHA-1 thumbprint) parameter is a base64url-encoded SHA-1 thumbprint (a.k.a. digest) of the DER encoding of an X.509 certificate [RFC5280]. Note that certificate thumbprints are also sometimes known as certificate fingerprints. The key in the certificate MUST match the public key represented by other members of the JWK. Use of this member is OPTIONAL.
  ls-type:: annotation
  hl-page:: 9
  hl-color:: blue
  id:: 658b1f8a-7fa5-41e2-9c10-3e77a721977f
- "x5t#S256" (X.509 Certificate SHA-256 Thumbprint) Parameter
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 658b1fad-3fcb-4775-9ce3-7180699357cd
- JWK Set Format
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 658b2019-3a4e-4fe8-9dd3-3be755a5b0df
- "keys" Parameter
  ls-type:: annotation
  hl-page:: 10
  hl-color:: blue
  id:: 658b2028-3570-493b-933c-0a865e80d5ab
- The string comparison rules for this specification are the same as those defined in Section 5.3 of [JWS].
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b2059-48af-47b6-b17d-a693f7722dcf
- Access to JWKs containing non-public key material by parties without legitimate access to the non-public information MUST be prevented. This can be accomplished by encrypting the JWK when potentially observable by such parties to prevent the disclosure of private or symmetric key values. The use of an Encrypted JWK, which is a JWE with the UTF-8 encoding of a JWK as its plaintext value, is recommended for this purpose.
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b2075-ad20-4ca5-823c-2724e33b1904
- The processing of Encrypted JWKs is identical to the processing of other JWEs. A "cty" (content type) Header Parameter value of "jwk+json" MUST be used to indicate that the content of the JWE is a JWK
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b2095-372e-4b91-94cb-a58a82cbd51e
- The use of an Encrypted JWK Set, which is a JWE with the UTF-8 encoding of a JWK Set as its plaintext value, is recommended for this purpose. The processing of Encrypted JWK Sets is identical to the processing of other JWEs. A"cty" (content type) Header Parameter value of "jwk-set+json" MUST be used to indicate that the content of the JWE is a JWK Set
  ls-type:: annotation
  hl-page:: 11
  hl-color:: blue
  id:: 658b20bb-60c5-472d-bc21-414dee67610e
- One should place no more trust in the data cryptographically secured by a key than in the method by which it was obtained and in the trustworthiness of the entity asserting an association with the key.
  ls-type:: annotation
  hl-page:: 20
  hl-color:: blue
  id:: 658b321c-3b0d-4b5d-8ae5-bb19d369b689
- applications make decisions about whether to trust a key based on attributes bound to the key, such as names, roles, and the key origin, rather than based on the key itself.
  ls-type:: annotation
  hl-page:: 20
  hl-color:: blue
  id:: 658b322f-f484-43dc-be10-07cf279450f1