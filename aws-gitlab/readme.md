# aws-gitlab toolkit

`Amazon Web Services` (aws) is an omnipresent cloud infrastructure provider in 2022.

`GitLab` is an all-in-on DevOps platform built over a centralized source code 
repository (`git`) and a powerful continuous integration and deployement pipeline.

## pain points

- developers quickly get chained to their deployment pipelines to develop new 
features or fix bugs.
- deploying to the cloud is time and money expensive
  - machines are required to run pipelines, build artifacts, and deploy them on 
   an cloud environment
  - pipeline runs are often long enough to make a developer remain idle, and quick 
    enough to not incentivise developers to work on something else in parallel

## optimize local development environments

Developers workstation are powerful enough to host one to many developing environments.

- test bug fixes
- run unit and end-to-end automated tests
- conduct experiments

### Docker

(explain how Docker/Docker desktop is the central tool to have a viable local 
 environment for cloud development)

### localstack

(explain how localstack is a viable alternative to `aws` in a local setting)

[https://localstack.cloud/](https://localstack.cloud/)

### run CI pipelines locally

GitLab CI pipeline development is centralized to a declarative manifest: `.gitlab-ci.yml`. 
This code is the backbone of any project built on the GitLab platform. However, 
developping and refactoring pipeline jobs can be a tedious task if you end up 
adopting the "trial and error" method; running pipelines on actual cloud resources.

Running pipelines locally and leveraging a cloud mocking platform such as `localstack` 
is promising.

#### firecow/gitlab-ci-local

(explain what it is)

(add pros and cons)

> "Tired of pushing to test your .gitlab-ci.yml?
>
> Run gitlab pipelines locally as shell executor or docker executor.
>
> Get rid of all those dev specific shell scripts and make files."

[https://github.com/firecow/gitlab-ci-local](https://github.com/firecow/gitlab-ci-local)

#### use actual gitlab-runner exec locally

(explain it)

(explain pros and cons.  especially versus firecow/gitlab-ci-local)

(todo: add better docs than a short blog post)

[https://medium.com/@umutuluer/how-to-test-gitlab-ci-locally-f9e6cef4f054](https://medium.com/@umutuluer/how-to-test-gitlab-ci-locally-f9e6cef4f054)