# php lab41
- deployment through AWS Codepipeline
- Authors: Trevor Dobson, Jack Daniel Kinne, Brandon Hurrington, Padmapriya Ganapathi.
- Challenge by: CodeFellows.

## Deployed link:
[link here](http://php-env.a5b8prwjvw.us-west-2.elasticbeanstalk.com/)


## Challenge
- Using only the instructions provided to you, implement a working CI/CD Pipeline
- Once you have it working …
- Add a “Build” stage to your Pipeline which includes the following steps (depending on your app)
- Build
- Test

## setup

Create Code pipleine.
### Step one:
create new service role
![step](step1.png)

### Step two:
Setup github repo as the source.
![step](step2.png)

### Step three:
- Choose repo
![step](step3.png)

### (there is no step four)
- This app does not require a build stage.

### Step five:
Choose application.  We recommend you choose the sample application at first, to confirm deployment works.
![step](step5.png)

### review
- Review your choices
![step](review.png)

### Success
You shoud now see a green pipeline.
![step](success.png)


## gotchas
- PROBLEM: in the buildspec.yml, ensure that PHP targets 7.2, as that is the latest version supported on the ENV for Elastic Beanstalk. DO NOT USE the class repo offering of the buildspec.yml file.
- SOLUTION: Ensure you are using an exact copy of the buildspec.yml included in this repo.

- You do not need a build.

## credits and contributions
- Jack Daniel Kinne
- Brandon Hurrington
- Padmapriya Ganapathi
- Trevor Dobson
- Steve Grant
- https://docs.aws.amazon.com/codebuild/latest/userguide/build-spec-ref.html#runtime-versions-buildspec-file

