# Harbor an open source trusted cloud native registry project that stores, signs, and scans content.

Harbor

Harbor is an open source trusted cloud native registry project that stores, signs, and scans content. Harbor extends the open source Docker Distribution by adding the functionalities usually required by users such as security, identity and management. Having a registry closer to the build and run environment can improve the image transfer efficiency. Harbor supports replication of images between registries, and also offers advanced security features such as user management, access control and activity auditing.

Harbor is hosted by the Cloud Native Computing Foundation (CNCF). If you are an organization that wants to help shape the evolution of cloud native technologies, consider joining the CNCF. For details about whose involved and how Harbor plays a role, read the CNCF announcement.
Features

    Cloud native registry: With support for both container images and Helm charts, Harbor serves as registry for cloud native environments like container runtimes and orchestration platforms.
    Role based access control: Users access different repositories through 'projects' and a user can have different permission for images or Helm charts under a project.
    Policy based replication: Images and charts can be replicated (synchronized) between multiple registry instances based on policies with using filters (repository, tag and label). Harbor automatically retries a replication if it encounters any errors. This can be used to assist loadbalancing, achieve high availability, and facilitate multi-datacenter deployments in hybrid and multi-cloud scenarios.
    Vulnerability Scanning: Harbor scans images regularly for vulnerabilities and has policy checks to prevent vulnerable images from being deployed.
    LDAP/AD support: Harbor integrates with existing enterprise LDAP/AD for user authentication and management, and supports importing LDAP groups into Harbor that can then be given permissions to specific projects.
    OIDC support: Harbor leverages OpenID Connect (OIDC) to verify the identity of users authenticated by an external authorization server or identity provider. Single sign-on can be enabled to log into the Harbor portal.
    Image deletion & garbage collection: System admin can run garbage collection jobs so that images(dangling manifests and unreferenced blobs) can be deleted and their space can be freed up periodically.
    Notary: Support signing container images using Docker Content Trust (leveraging Notary) for guaranteeing authenticity and provenance. In addition, policies that prevent unsigned images from being deployed can also be activated.
    Graphical user portal: User can easily browse, search repositories and manage projects.
    Auditing: All the operations to the repositories are tracked through logs.
    RESTful API: RESTful APIs are provided to facilitate administrative operations, and are easy to use for integration with external systems. An embedded Swagger UI is available for exploring and testing the API.
    Easy deployment: Harbor can be deployed via Docker compose as well Helm Chart, and a Harbor Operator was added recently as well.

Architecture

For learning the architecture design of Harbor, check the document Architecture Overview of Harbor.
API

    Harbor RESTful API: The APIs for most administrative operations of Harbor and can be used to perform integrations with Harbor programmatically.
        Part 1: New or changed APIs

Install & Run

System requirements:

On a Linux host: docker 20.10.10-ce+ and docker-compose 1.18.0+ .

Download binaries of Harbor release and follow Installation & Configuration Guide to install Harbor.

If you want to deploy Harbor on Kubernetes, please use the Harbor chart.

Refer to the documentation for more details on how to use Harbor.
OCI Distribution Conformance Tests

Check the OCI distribution conformance tests report of Harbor.
Compatibility

The compatibility list document provides compatibility information for the Harbor components.

    Replication adapters
    OIDC adapters
    Scanner adapters

Community

    Twitter: @project_harbor
    User Group: Join Harbor user email group: harbor-users@lists.cncf.io to get update of Harbor's news, features, releases, or to provide suggestion and feedback.
    Developer Group: Join Harbor developer group: harbor-dev@lists.cncf.io for discussion on Harbor development and contribution.
    Slack: Join Harbor's community for discussion and ask questions: Cloud Native Computing Foundation, channel: #harbor and #harbor-dev

Demos

    Live Demo - A demo environment with the latest Harbor stable build installed. For additional information please refer to this page.
    Video Demos - Demos for Harbor features and continuously updated.

Partners and Users

For a list of users, please refer to ADOPTERS.md.
Security
Security Audit

A third party security audit was performed by Cure53 in October 2019. You can see the full report here.
Reporting security vulnerabilities

If you've found a security related issue, a vulnerability, or a potential vulnerability in Harbor please let the Harbor Security Team know with the details of the vulnerability. We'll send a confirmation email to acknowledge your report, and we'll send an additional email when we've identified the issue positively or negatively.

For further details please see our complete security release process.
License

Harbor is available under the Apache 2 license.

This project uses open source components which have additional licensing terms. The official docker images and licensing terms for these open source components can be found at the following locations:

    Photon OS 1.0: docker image, license
