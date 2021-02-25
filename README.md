# angular_thebusiness_ui
Project created for my friend entrepreneurship, also I expect this to be a great exercise for my web development skill and some docker tricks.

I dont linke installing software in my machine, so lest download a angular machine capable of using ng-cli, this one https://hub.docker.com/r/trion/ng-cli-karma.

Acording to the documentation, I need the docker IMAGE ID to execute the creation of my angular project

docker run -u $(id -u) --rm -v "$PWD":/app trion/ng-cli-karma ng new BussinessUI

cd BussinessUI

docker run -p 4200:4200 -u $(id -u) --rm -v "$PWD":/app trion/ng-cli-karma ng serve --host 0.0.0.0
