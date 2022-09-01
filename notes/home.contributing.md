---
id: x84sn91kbhdc7wwc58m3ho0
title: Contributing
desc: ''
updated: 1661817895828
created: 1661811133582
homepage: https://dendronhq.github.io/cascadia-js-2022/
---

# Day 1

## **The Web Is Good Now: Chris Coyier ("Shop Talk" podcast)**

### Layout:

  grid masonory
  css container queries

### Images:

- flip
- cloudinary.com/{formatting-optimization parameters}/{location of URL}
  use ^^ link in website so that the optimized, formatted image is used

- Web Font/Typography:
  - font-display: swap
  - font-display: optional

### Typography
- variable fonts  / ie: roboto-flex
  - pass 'font-variation-seetings to a class.
- fluid type


- Container units:
    container utins (ie: 'qw') allows you to assign font sizes that are scoped relative to the container


## **Enhance your Functional Web Apps with Web Components: Brian Leroux**

[enhance.dev](https://enhance.dev/docs/)

Progressinge enhancement
- ethical case (good for all people)
- busness case (good for more people === more $$)
- developer case (better experiece for devs)

ENHANCE - the product Brian is selling.
- HTML framework
- author HTML and progressivley enhance with JS/backend functions
<br>
<br>

### Projuct Fugo
- google let attempt to match native UX on web
- Why not know better?
  - Apple (hopefully resolved by anti-trust suites)
  - Official docs are _bleh_
- https://developer.chrome.com/blog/fugu-showcase/
- can i use: webUSB

### Wbauthn aka FIDO2
- moving away from password
- moving towards biometrics/ub key
- https://webauthn.guide/

### Share API
- shareAPI

### WebUSB

### File System Access API (Photoshop)
web-dev/ps-on-the-web

### ML-driven UX
https://teachablemachine.withgoogle.com
<br>
<br>


## Doing Data as a Frontend Developer: Tejas Kumar

### "Data": what is it?
- data in the browser (ie: local storage, indexDB)
  - unable to share across platforms/instances
- data in the cloud.  ("The Backend")
- The Database: Relational vs. Non-relational
### Relational
- structured language
- normalization
- ACID (an acronym representing transactional gaurantees in the relational model)
  - Atomicity: a single unit of work
  - Consistency
  - isolation
  - Durability
- Limitations
  - vertical scaling
### Non-Relational
- built for scale
- key/value stores
- unstructured
- partitionable
- BASE
  - Basically Available
  - Soft State
  - Eventually Consistent
### New SQL: The best of both worlds
- Aurora
- Fuana
- xeta

Why not use both?
Data infastructure > database
<br>
<br>

## **The 90s Called and They Want Their Websites Back**: Rachel White
<br><br>

## **Publishing in the JavaScript Ecosystem & Keeping Users Happy** Trivikram Kamat

- support only modern browsers
- server: support node.js with optional deno/clouflare workers support
- JS native: it depends
- module formats: dual package CJS+ESM, optional ESM only variant
- sizes: aim for smaler publish/install.bundle sizes
- types: at least puhlish typescript types.
- derubgging: provide sources

<br>
<br>

## **Cryptography Isn't Scary**: Eddie Zaneski

### TERMS
- semetric key: single key
- awymmetric (public/private keys)
- one-way functions: easy to init. hard to reverse
- psuedo-random number generator
- modular arithmetic

### KEYS
- RSA - outdated
- ECC: ecliptic curve computations

### Diffie Hellman Key Exhange
- aes symetric key
- used to create handshakes on internet
  - the classic public/private paint exhange examples

### Web Crypto API
  - getRandomValues(TypedArray)
  - SubtleCrypto

### NSA Backdoor
- NSA tried to push random number generator Dual_EC_DRBG
- confirmed by Snowden link.  Read about it.

### Sigstore
- new standard for signing, verifying, and protecthing software
- https://sigstore.dev
- "keyless" signing (Fulcio)
- Transparency log (Rekor)
- sigstore.js
- https://github.com/sigstore/sigstore-js
- npm-rfc
<br>
<br>

## **Reverse Engineering a Private API**: Joyce Lin

### Why reverse engineer APIs
- lots of reasons
  - kudos / personal gain / malicious intent / cred
- be ethical.
- understand legal ramifications

### Capturing network traffic
- copy a network request as a curl
- execute the curl and inspect the returned data
- can also save session data as curl

### Capturing session data as har file
- save all as har with content
- import har file

### Capture stream of HTTP API
- free web proxy tools
  - postman
  - mitproxy 
  - ...more
- use proxy server to capture network traffic
  - postman has a browser extension that can do this (Interceptor)

### Replay API calls
- cookie based auth
- can use 'google-bot' as a user-agent to spoof client-attributes
- Replay in code:
