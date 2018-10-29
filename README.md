# elastisys-pom-public

This POM file is intended for Elastisys Java projects that are to be deployed to
Maven central and (optionally) build Docker images published in Docker Hub.


## Deploying

To release a new version of the POM, run the `release.sh` script. This
script will prompt you for the new version number, automatically tag and
push the changes to the remote git repository and deploy the POM file to 
Maven central.

**NOTE** that _after_ deploying to the staging repository, you need to head to
https://oss.sonatype.org/#stagingRepositories and approve the release. Go to
staging repositories, search for `elastisys` or similar to find the released
repository. Then "Close" the repository (takes some time, you may need to
refresh) and finally "Release" the repository. Only after this step has been
completed will the released artifacts show up in the public Maven repo under
https://oss.sonatype.org/content/groups/public/com/elastisys/.
