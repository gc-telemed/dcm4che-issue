# Issue Details

This repo contains files that might be relevant for resolving the dcm4che issue regarding DICOM study folder not getting loaded into dcm4che.

After dcm4che and OHIF viewer were setup without any docker build issues,the following command was run:

```
docker run -v /home/myuser/Documents/dicom-data:/tmp --rm --network=nginxdcm4che_dcm4che_default dcm4che/dcm4che-tools:5.14.0 storescu -c DCM4CHEE@arc:11112 /tmp 1>>docker-storescu.log 2>>docker-storescu.err.log
```

The stdout and stderr files are in the repo.

Also included are docker config files and the output from

```
storescu -c DCM4CHEE@localhost:11112 . 1>>storescu.log 2>>storescu.err.log
```

Other files, if relevant will be added here.