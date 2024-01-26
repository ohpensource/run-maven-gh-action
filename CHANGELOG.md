# :confetti_ball: 0.10.0 (2024-01-26T13:20:38.048Z)
- - -
## :hammer: Features
* CMM-22507 always show full stack-trace of error
## :newspaper: Others
* docs: CMM-22507 remove empty line
- - -
- - -
# :confetti_ball: 0.9.0 (2023-09-28T09:07:14.376Z)
- - -
## :hammer: Features
* HUBSA-2346 added back AWS_PROFILE which is used in StsAssumeRoleCredentialsProvider and in old OhpenMavenPlugin and DVPCOMMONS maven plugins (#13)
- - -
- - -
# :confetti_ball: 0.8.0 (2023-09-27T10:01:52.632Z)
- - -
## :hammer: Features
* HUBSA-2346 use PLUGINS_AWS_PROFILE instead of standard AWS_PROFILE (used internally by AWS SDK v1 and v2) for avoid problems in OhpenMavenPlugins
## :newspaper: Others
* docs: HUBSA-2346 added hint about PLUGINS_AWS_PROFILE to README file
- - -
- - -
# :confetti_ball: 0.7.0 (2023-07-12T10:09:15.804Z)
- - -
## :hammer: Features
* PE-2328 include also number of CPU cores in calculation of available memory used by maven
## :newspaper: Others
* docs: PE-2328 added description for threads input parameter into README file
* docs: PE-2328 update comments for memory calculation
- - -
- - -
# :confetti_ball: 0.6.0 (2023-06-21T12:50:52.946Z)
- - -
## :hammer: Features
* HUBSA-2362 pass proper profiles to maven build
* HUBSA-2362 removed dots
- - -
- - -
# :confetti_ball: 0.5.0 (2023-03-22T11:08:45.008Z)
- - -
## :hammer: Features
* DOCS-2044 fixed deprecated github commands (#9)
- - -
- - -
# :confetti_ball: 0.4.1 (2023-02-08T15:46:03.549Z)
- - -
## :bug: Fixes
* CRA-2903 fixed bad setting of step output
* CRA-2903 empty readme change
- - -
- - -
# :confetti_ball: 0.4.0 (2023-02-08T10:24:05.481Z)
- - -
## :hammer: Features
* CRA-2903 added step for determining additional maven arguments based on build-modules
* CRA-2903 PR improvements
- - -
- - -
# :confetti_ball: 0.3.0 (2023-01-16T08:46:39.963Z)
- - -
## :hammer: Features
* OIMP-190 update GH actions versions
## :newspaper: Others
* docs: OIMP-190 empty line
- - -
- - -
# :confetti_ball: 0.2.1 (2022-05-03T10:44:02.094Z)
- - -
## :bug: Fixes
* CLIC-7519 remove memory for system
## :newspaper: Others
* docs: CLIC-7519 added documentation for "save-cache" input parameter
- - -
- - -
# :confetti_ball: 0.2.0 (2022-04-29T13:31:48.953Z)
- - -
## :hammer: Features
* CLIC-7519 define credentials environment variables for AWS SDK v1 and v2
* CLIC-7519 automatically calculate maximal available memory form maven process
## :bug: Fixes
* CLIC-7519 put MAVEN_OPTS to GITHUB_ENV file
* CLIC-7519 remove echo comment which print Maven options information - stored into GITHUB_ENV
## :newspaper: Others
* docs: CLIC-7519 documentation for added credentials environment variables for AWS SDK v1 and v2
- - -
- - -
# :confetti_ball: 0.1.0 (2022-04-13T09:30:07.692Z)
- - -
## :hammer: Features
* CLIC-7519 added jvm-options configuration which will be used as MAVEN_OPTS
## :newspaper: Others
* style:CLIC-7519 added GIT ignore for IntelliJ IDEA files
* docs:CLIC-7519 added description for new jvm-options input to README file
- - -
- - -
# :confetti_ball: 0.0.1 (2022-04-07T17:18:24.268Z)
- - -
## :newspaper: Others
* Merge pull request #1 from ohpensource/LANZ-2217
- - -
- - -
