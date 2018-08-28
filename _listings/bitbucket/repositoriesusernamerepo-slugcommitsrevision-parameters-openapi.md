---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Commits Revision
  description: Parameters repositories username repo slug commits revision
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/commit/{revision}:
    get:
      summary: Get Repositories Username Repo Slug Commit Revision
      description: Get repositories username repo slug commit revision
      operationId: getRepositoriesUsernameRepoSlugCommitRevision
      x-api-path-slug: repositoriesusernamerepo-slugcommitrevision-get
      parameters:
      - in: path
        name: revision
        description: The commits SHA1
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Revision
    parameters:
      summary: Parameters Repositories Username Repo Slug Commit Revision
      description: Parameters repositories username repo slug commit revision
      operationId: parametersRepositoriesUsernameRepoSlugCommitRevision
      x-api-path-slug: repositoriesusernamerepo-slugcommitrevision-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Revision
  /repositories/{username}/{repo_slug}/commits/{revision}:
    get:
      summary: Get Repositories Username Repo Slug Commits Revision
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
      operationId: getRepositoriesUsernameRepoSlugCommitsRevision
      x-api-path-slug: repositoriesusernamerepo-slugcommitsrevision-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commits
      - Revision
    parameters:
      summary: Parameters Repositories Username Repo Slug Commits Revision
      description: Parameters repositories username repo slug commits revision
      operationId: parametersRepositoriesUsernameRepoSlugCommitsRevision
      x-api-path-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commits
      - Revision
    post:
      summary: Add Repositories Username Repo Slug Commits Revision
      description: |-
        Identical to `GET /repositories/{username}/{repo_slug}/commits`,
        except that POST allows clients to place the include and exclude
        parameters in the request body to avoid URL length issues.

        **Note that this resource does NOT support new commit creation.**
      operationId: postRepositoriesUsernameRepoSlugCommitsRevision
      x-api-path-slug: repositoriesusernamerepo-slugcommitsrevision-post
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commits
      - Revision
  /snippets/{username}/{encoded_id}/commits/{revision}:
    get:
      summary: Get Snippets Username Encoded  Commits Revision
      description: Get snippets username encoded  commits revision
      operationId: getSnippetsUsernameEncodedCommitsRevision
      x-api-path-slug: snippetsusernameencoded-idcommitsrevision-get
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Commits
      - Revision
    parameters:
      summary: Parameters Snippets Username Encoded  Commits Revision
      description: Parameters snippets username encoded  commits revision
      operationId: parametersSnippetsUsernameEncodedCommitsRevision
      x-api-path-slug: snippetsusernameencoded-idcommitsrevision-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Commits
      - Revision
  /snippets/{username}/{encoded_id}/{revision}/diff:
    get:
      summary: Get Snippets Username Encoded  Revision Diff
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
      operationId: getSnippetsUsernameEncodedRevisionDiff
      x-api-path-slug: snippetsusernameencoded-idrevisiondiff-get
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      - in: query
        name: path
        description: When used, only one the diff of the specified file will be returned
      - in: path
        name: revision
        description: A revspec expression
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Diff
    parameters:
      summary: Parameters Snippets Username Encoded  Revision Diff
      description: Parameters snippets username encoded  revision diff
      operationId: parametersSnippetsUsernameEncodedRevisionDiff
      x-api-path-slug: snippetsusernameencoded-idrevisiondiff-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Diff
  /snippets/{username}/{encoded_id}/{revision}/patch:
    get:
      summary: Get Snippets Username Encoded  Revision Patch
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
      operationId: getSnippetsUsernameEncodedRevisionPatch
      x-api-path-slug: snippetsusernameencoded-idrevisionpatch-get
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      - in: path
        name: revision
        description: A revspec expression
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Patch
    parameters:
      summary: Parameters Snippets Username Encoded  Revision Patch
      description: Parameters snippets username encoded  revision patch
      operationId: parametersSnippetsUsernameEncodedRevisionPatch
      x-api-path-slug: snippetsusernameencoded-idrevisionpatch-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Revision
      - Patch
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---