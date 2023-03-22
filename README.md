# setup-maven-gh-action

* Action runs maven command with supplied parameters. 
* Includes saving cache after build. 
* In case that build needs to assume aws role use optional parameter: maven-aws-role.
    * Maven step configure credentials environment variables for **AWS SDK v1/v2** and _AWS_ASSUME_ROLE_ARN_ for assume role credentials provider

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

**Note:**

This action: [https://github.com/skjolber/maven-cache-github-action] was replaced by equivalent fork with fixed
deprecated GitHub commands and node version. If original repo action will be fixed, we can move to new version.

# Advanced settings

* _save-cache_ - If cache should be saved after maven run
* _jvm-options_ - Maven Java virtual machine settings like memory configuration
    * if missing JVM **-Xmx** parameter then action automatically calculate maximally available memory for maven process
* _build-dependant-modules_ - Use [true] for argument _--also-make-dependents_, [false] for argument _--also-make_

# License Summary

This code is made available under the MIT license. Details [here](LICENSE).
