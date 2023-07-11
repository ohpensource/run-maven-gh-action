# setup-maven-gh-action

* Action runs maven command with supplied parameters. 
* Includes saving cache after build. 
* Maven run command uses: **maven-aws-profile** for running build. 
* It sets also environment variables to be backward compatible with AWS SDK v.1.
** for this purpose is used **plugins-aws-profile** if not set, then: **maven-aws-profile**

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
```

# Advanced settings

* _save-cache_ - If cache should be saved after maven run
* _jvm-options_ - Maven Java virtual machine settings like memory configuration
    * if missing JVM **-Xmx** parameter then action automatically calculate maximally available memory for maven process
* _threads_ - Maven thread parameter: eg. 1.5C, 1C, 4. Default 1 thread pre CPU core
    * if missing JVM **-Xmx** parameter then number of CPU cores are included into calculation of maximally available memory for maven process
    * if there is use "[0-9.]C" setting then all available CPU cores are used
* _build-dependant-modules_ - Use [true] for argument _--also-make-dependents_, [false] for argument _--also-make_

# License Summary

This code is made available under the MIT license. Details [here](LICENSE).
