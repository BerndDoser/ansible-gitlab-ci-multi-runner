ansible-gitlab-ci-multi-runner
==============================

Install and register a GitLab-CI multi-runner

Requirements
------------

Create a registration token on the admin/runners page of your GitLab instance.

Role Variables
--------------

 - gitlab_ci_multi_runner_executor (default: docker)
 - gitlab_ci_multi_runner_name (default: docker-runner)
 - gitlab_ci_multi_runner_url
 - gitlab_ci_multi_runner_registration_token

Dependencies
------------

None.

Example Playbook
----------------

```groovy
  - hosts: all
    roles:
      - { role: bernddoser.ansible-gitlab-ci-multi-runner, gitlab_ci_multi_runner_url: <gitlab url>, gitlab_ci_multi_runner_registration_token: <registration token> }
```

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
