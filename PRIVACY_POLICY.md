# Checkmater Privacy Policy

Effective date: March 27, 2026

This Privacy Policy applies to the Checkmater plugin for JetBrains products ("Checkmater", "the Plugin").

## 1. Summary

Checkmater can work in two different ways:

- Local puzzle features store limited settings and gameplay progress on the user's machine.
- Optional online features can send data to a configured backend server if the user signs in or uses networked gameplay features.

## 2. Data Stored Locally

Based on the current codebase, the Plugin stores the following local data:

- plugin settings and gameplay progress, including preferred puzzle mode, solved levels, streak, best streak, total attempts, and configured backend URL;
- authentication state for optional online features, stored through JetBrains Password Safe when the user signs in.

Local settings are stored by the JetBrains platform in the IDE configuration environment. Authentication credentials and tokens are stored through JetBrains Password Safe rather than plain text project files.

## 3. Data Sent Over Network

If the user enables or uses online features, the Plugin may send data to the configured backend server, including:

- username and password during registration or login;
- refresh tokens and access tokens for session handling;
- profile requests, game actions, room codes, queue participation, challenges, and gameplay events;
- WebSocket messages required for live online features.

The current codebase uses a configurable backend base URL and defaults to `http://localhost:8080`.

## 4. What Checkmater Does Not Claim

Checkmater does not claim to collect analytics, advertising identifiers, or telemetry in the currently verified code paths reviewed for this policy.

This statement is limited to the code verified in the repository as of March 27, 2026. If the Plugin is changed later, this policy should be updated accordingly.

## 5. Backend Operator Responsibility

If online features are used, data may be processed by the operator of the backend server configured by the user or bundled by the Plugin distributor.

The Plugin codebase includes server-side models for accounts, ratings, match history, and related gameplay data, but actual server deployment, retention, logging, and infrastructure practices depend on the backend operator.

If you run or provide a public backend for Checkmater, you are responsible for publishing any additional service-specific privacy disclosures that apply to that backend.

## 6. Legal Basis and User Choice

Use of local-only features is optional. Use of online features is also optional and initiated by the user.

If a user does not want network processing, they should avoid registration, login, and other online gameplay features, and use only local puzzle functionality.

## 7. Data Security

Checkmater relies in part on JetBrains platform facilities such as Password Safe for credential storage. No security method is guaranteed to be perfect, and use of the Plugin is at the user's own risk.

## 8. Data Retention

Local settings remain on the user's machine until removed by the user, the IDE, or normal configuration cleanup.

Server-side retention for optional online features is determined by the backend operator and is not fully defined by the Plugin alone.

## 9. Children's Privacy

Checkmater is not directed specifically to children. Do not use online features if you are not permitted to share account information under applicable law.

## 10. International Use

Users may run the Plugin and any backend in different countries. If online features are used, data may be transferred to and processed in the country where the configured backend operates.

## 11. Changes to This Policy

This Privacy Policy may be updated when the Plugin or its data practices change. The effective date above should also be updated when changes are made.

## 12. Contact

For privacy questions related to this repository, use the repository contact point or issue tracker:

- `git@github.com:zhaksyaslan/Checkmater.git`
