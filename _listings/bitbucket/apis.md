---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Revisions
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
  description: Parameters repositories username repo slug commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-get
  description: Get snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-parameters
  description: Parameters snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-get
  description: |-
    Returns the diff of the specified commit against its first parent.

    Note that this resource is different in functionality from the `patch`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the diff is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-parameters
  description: Parameters snippets username encoded  revision diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-get
  description: |-
    Returns the patch of the specified commit against its first
    parent.

    Note that this resource is different in functionality from the `diff`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the patch is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-parameters
  description: Parameters snippets username encoded  revision patch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
  description: Parameters repositories username repo slug commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-get
  description: Get snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-parameters
  description: Parameters snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-get
  description: |-
    Returns the diff of the specified commit against its first parent.

    Note that this resource is different in functionality from the `patch`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the diff is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-parameters
  description: Parameters snippets username encoded  revision diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-get
  description: |-
    Returns the patch of the specified commit against its first
    parent.

    Note that this resource is different in functionality from the `diff`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the patch is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-parameters
  description: Parameters snippets username encoded  revision patch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-parameters
  description: Parameters snippets username encoded  revision patch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Patch
  x-api-slug: snippetsusernameencoded-idrevisionpatch-get
  description: |-
    Returns the patch of the specified commit against its first
    parent.

    Note that this resource is different in functionality from the `diff`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the patch is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisionpatch-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-parameters
  description: Parameters snippets username encoded  revision diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Revision Diff
  x-api-slug: snippetsusernameencoded-idrevisiondiff-get
  description: |-
    Returns the diff of the specified commit against its first parent.

    Note that this resource is different in functionality from the `patch`
    resource.

    The differences between a diff and a patch are:

    * patches have a commit header with the username, message, etc
    * diffs support the optional `path=foo/bar.py` query param to filter the
      diff to just that one file diff (not supported for patches)
    * for a merge, the diff will show the diff between the merge commit and
      its first parent (identical to how PRs work), while patch returns a
      response containing separate patches for each commit on the second
      parent's ancestry, up to the oldest common ancestor (identical to
      its reachability).

    Note that the character encoding of the contents of the diff is
    unspecified as Git and Mercurial do not track this, making it hard for
    Bitbucket to reliably determine this.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idrevisiondiff-get-openapi.md
- name: Bitbucket - Parameters Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-parameters
  description: Parameters snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-parameters-openapi.md
- name: Bitbucket - Get Snippets Username Encoded  Commits Revision
  x-api-slug: snippetsusernameencoded-idcommitsrevision-get
  description: Get snippets username encoded  commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/snippetsusernameencoded-idcommitsrevision-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
  description: Parameters repositories username repo slug commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/revisions/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---