
<p align="center" style="margin-bottom: 0px !important;">
  <img width="256" src="https://raw.githubusercontent.com/minkan-chat/brand/main/assets/3d/logo-borders%40512.png" alt="Material Bread logo" align="center">
</p>
<h1 align="center" style="margin-top: 0px;">Minkan</h1>

<p align="center">A end-to-end encrypted zero-trust capable messaging platform</p>

## Architecture

Minkan combines existing, well-established as well as new technologies into one platform. 

The core of Minkan is the concept of a [web of trust] so users (clients) do not have to rely on a 
central authority (e.g. a server) to provide the correct identity for an user. For that, Minkan uses [OpenPGP].

Minkan uses the OpenPGP identities with messaging protocols to achieve forward secrecy and post-compromise security.
For one-to-one communication, Minkan uses the [Signal protocol]. For groups, Minkan aims to use [Messaging Layer Security (MLS)].

For the communication with the server, Minkan uses a [GraphQL] API.

Minkan uses [CBOR] as data format in the GraphQL API as well as in the actual client packets used in the client-to-client communication.
This enables clients to be versionless.

For authentication (in the client-to-server context), Minkan relies on an [OpenID Connect] provider with [Back-Channel Logout] support.

[web of trust]: https://en.wikipedia.org/wiki/Web_of_trust
[OpenPGP]: https://www.openpgp.org/
[Signal protocol]:https://signal.org/docs/
[Messaging Layer Security (MLS)]: https://messaginglayersecurity.rocks/
[GraphQL]: https://graphql.org/
[CBOR]: https://cbor.io/
[OpenID Connect]: https://openid.net/connect/
[Back-Channel Logout]: https://openid.net/specs/openid-connect-backchannel-1_0.html
