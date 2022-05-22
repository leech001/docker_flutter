# Docker compose and Ubuntu Linux images for Flutter &amp; Dart

Add this repository to the root of your flutter project.
Go to the 'you_flutter_project/docker/linux-build' directory and run the command
```
docker-compose up
```
The results of building your application will be in the 'you_flutter_project/build' folder of your project.

If you need to build a linux application with the 'system_tray' package (https://pub.dev/packages/system_tray) go to the directory './docker/linux-build' and open the Dockerfile and uncheck the corresponding comment to include the additional libraries in the image build.