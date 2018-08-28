---
name: Firebase
x-slug: firebase
description: Firebase is a mobile platform that gives developers the tools and infrastructure
  to build better apps and grow successful businesses.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
x-kinRank: "9"
x-alexaRank: "1"
tags: Releases
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/apis.md
specificationVersion: "0.14"
apis:
- name: Firebase - Delete Release
  x-api-slug: v1name-delete
  description: Delete a `Release` by resource name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-delete-openapi.md
- name: Firebase - Get Release
  x-api-slug: v1name-get
  description: Get a `Release` by name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-get-openapi.md
- name: Firebase - Update Release
  x-api-slug: v1name-put
  description: |-
    Update a `Release`.

    Only updates to the `ruleset_name` field will be honored. `Release` rename
    is not supported. To create a `Release` use the CreateRelease method
    instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-put-openapi.md
- name: Firebase - List Releases
  x-api-slug: v1namereleases-get
  description: |-
    List the `Release` values for a project. This list may optionally be
    filtered by `Release` name or `Ruleset` id or both.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-get-openapi.md
- name: Firebase - Create Releases
  x-api-slug: v1namereleases-post
  description: |-
    Create a `Release`.

    Release names should reflect the developer's deployment practices. For
    example, the release name may include the environment name, application
    name, application version, or any other name meaningful to the developer.
    Once a `Release` refers to a `Ruleset`, the rules can be enforced by
    Firebase Rules-enabled services.

    More than one `Release` may be 'live' concurrently. Consider the following
    three `Release` names for `projects/foo` and the `Ruleset` to which they
    refer.

    Release Name                    | Ruleset Name
    --------------------------------|-------------
    projects/foo/releases/prod      | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/beta | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/v23  | projects/foo/rulesets/uuid456

    The table reflects the `Ruleset` rollout in progress. The `prod` and
    `prod/beta` releases refer to the same `Ruleset`. However, `prod/v23`
    refers to a new `Ruleset`. The `Ruleset` reference for a `Release` may be
    updated using the UpdateRelease method, and the custom `Release` name
    may be referenced by specifying the `X-Firebase-Rules-Release-Name` header.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-post-openapi.md
- name: Firebase - Delete Release
  x-api-slug: v1name-delete
  description: Delete a `Release` by resource name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-delete-openapi.md
- name: Firebase - Get Release
  x-api-slug: v1name-get
  description: Get a `Release` by name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-get-openapi.md
- name: Firebase - Update Release
  x-api-slug: v1name-put
  description: |-
    Update a `Release`.

    Only updates to the `ruleset_name` field will be honored. `Release` rename
    is not supported. To create a `Release` use the CreateRelease method
    instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-put-openapi.md
- name: Firebase - List Releases
  x-api-slug: v1namereleases-get
  description: |-
    List the `Release` values for a project. This list may optionally be
    filtered by `Release` name or `Ruleset` id or both.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-get-openapi.md
- name: Firebase - Create Releases
  x-api-slug: v1namereleases-post
  description: |-
    Create a `Release`.

    Release names should reflect the developer's deployment practices. For
    example, the release name may include the environment name, application
    name, application version, or any other name meaningful to the developer.
    Once a `Release` refers to a `Ruleset`, the rules can be enforced by
    Firebase Rules-enabled services.

    More than one `Release` may be 'live' concurrently. Consider the following
    three `Release` names for `projects/foo` and the `Ruleset` to which they
    refer.

    Release Name                    | Ruleset Name
    --------------------------------|-------------
    projects/foo/releases/prod      | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/beta | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/v23  | projects/foo/rulesets/uuid456

    The table reflects the `Ruleset` rollout in progress. The `prod` and
    `prod/beta` releases refer to the same `Ruleset`. However, `prod/v23`
    refers to a new `Ruleset`. The `Ruleset` reference for a `Release` may be
    updated using the UpdateRelease method, and the custom `Release` name
    may be referenced by specifying the `X-Firebase-Rules-Release-Name` header.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-post-openapi.md
- name: Firebase - Delete Release
  x-api-slug: v1name-delete
  description: Delete a `Release` by resource name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-delete-openapi.md
- name: Firebase - Get Release
  x-api-slug: v1name-get
  description: Get a `Release` by name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-get-openapi.md
- name: Firebase - Update Release
  x-api-slug: v1name-put
  description: |-
    Update a `Release`.

    Only updates to the `ruleset_name` field will be honored. `Release` rename
    is not supported. To create a `Release` use the CreateRelease method
    instead.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1name-put-openapi.md
- name: Firebase - List Releases
  x-api-slug: v1namereleases-get
  description: |-
    List the `Release` values for a project. This list may optionally be
    filtered by `Release` name or `Ruleset` id or both.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-get-openapi.md
- name: Firebase - Create Releases
  x-api-slug: v1namereleases-post
  description: |-
    Create a `Release`.

    Release names should reflect the developer's deployment practices. For
    example, the release name may include the environment name, application
    name, application version, or any other name meaningful to the developer.
    Once a `Release` refers to a `Ruleset`, the rules can be enforced by
    Firebase Rules-enabled services.

    More than one `Release` may be 'live' concurrently. Consider the following
    three `Release` names for `projects/foo` and the `Ruleset` to which they
    refer.

    Release Name                    | Ruleset Name
    --------------------------------|-------------
    projects/foo/releases/prod      | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/beta | projects/foo/rulesets/uuid123
    projects/foo/releases/prod/v23  | projects/foo/rulesets/uuid456

    The table reflects the `Ruleset` rollout in progress. The `prod` and
    `prod/beta` releases refer to the same `Ruleset`. However, `prod/v23`
    refers to a new `Ruleset`. The `Ruleset` reference for a `Release` may be
    updated using the UpdateRelease method, and the custom `Release` name
    may be referenced by specifying the `X-Firebase-Rules-Release-Name` header.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: Data, Real Time, API Provider, API Service Provider, SDIO Competition, Databases,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/releases/master/_listings/firebase/v1namereleases-post-openapi.md
x-common:
- type: x-google-firebase
  url: Hacker News Search
- type: x-stack-exchange-search
  url: Google Firebase
- type: x-website
  url: https://Firebase.google.com
- type: x-api-gallery
  url: http://fire.browse.api.gallery.streamdata.io
- type: x-api-stack
  url: http://firebase.stack.network
- type: x-blog
  url: https://firebase.googleblog.com/
- type: x-blog-rss
  url: http://firebase.googleblog.com/feeds/posts/default?alt=rss
- type: x-case-studies
  url: https://firebase.google.com/customers/
- type: x-change-log
  url: https://firebase.google.com/support/releases
- type: x-code
  url: https://firebase.google.com/docs/libraries/
- type: x-crunchbase
  url: https://crunchbase.com/organization/google
- type: x-documentation
  url: https://firebase.google.com/docs/
- type: x-faq
  url: https://firebase.google.com/support/faq/
- type: x-forum
  url: https://groups.google.com/forum/#!forum/firebase-talk
- type: x-github
  url: https://github.com/firebase
- type: x-pricing
  url: https://firebase.google.com/pricing/
- type: x-pricing
  url: https://adwords.google.com/home/pricing/
- type: x-slack
  url: https://firebase.community/
- type: x-submit-bug
  url: https://firebase.google.com/support/contact/bugs-features
- type: x-support
  url: https://firebase.google.com/support/
- type: x-twitter
  url: https://twitter.com/Google
- type: x-twitter
  url: https://twitter.com/firebase
- type: x-website
  url: https://firebase.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---