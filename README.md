# setup-maven-gh-action

* Action runs maven command with supplied parameters. 
* Includes saving cache after build. 
* In case that build needs to assume aws role use optional parameter: maven-aws-role.

```yaml
      - uses: ohpensource/run-maven-gh-action@v0.1.0
        name: Run maven command
        with:
          phases: clean install
          profiles: github
          parameters: >- 
            -DuseGitHub=true
            -Denable.deploy=false
          threads: 1C
          save-cache: true
          maven-aws-access-key: <<AWS_ACCESS_KEY>>
          maven-aws-secret-key: <<AWS_SECRET_KEY>>
          maven-aws-role: <<AWS_ROLE_TO_ASSUME>>
```

# License Summary

This code is made available under the MIT license. Details [here](LICENSE).