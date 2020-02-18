
# cs400-S2020-participations_repo

Designed for use with [GitHub Classroom](https://classroom.github.com/), this repository contains the starter files for this participation.

![Logo](graphics/cs400.png)

## Introduction

The student will be committing participations in this directory.

## Learning

If you have not done so already, please read all of the relevant [GitHub Guides](https://guides.github.com/) that explain how to use many of the features that GitHub provides. In particular, please make sure that you have read the following GitHub guides: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/), [Hello World](https://guides.github.com/activities/hello-world/), and [Documenting Your Projects on GitHub](https://guides.github.com/features/wikis/). Each of these guides will help you to understand how to use both [GitHub](http://github.com) and [GitHub Classroom](https://classroom.github.com/).

## Using GatorGrader to verify the submission
For this assignment you can use you can use the [GatorGrader
tool](https://github.com/GatorEducator/gatorgrader) run in another Docker container
to verify that the minimal content of your programs and a reflection document satisfies the requirements specified in the lab assignment sheet. Once you have finished the implementation of all programs and before you make your final submission, run the GatorGrader application to start `gradle grade` as a containerized application, using the [DockaGator](https://github.com/GatorEducator/dockagator) Docker image available on
[DockerHub](https://cloud.docker.com/u/gatoreducator/repository/docker/gatoreducator/dockagator).
First, to ensure that the following command will work correctly, you must create the cache directory by running the command `mkdir $HOME/.dockagator`. Then, to see if your submission satisfies the minimal requirements, you can run the below command in the terminal.

Linux or MacOS, putting the command all one line,

```
sudo docker run --rm --name dockagator  -v "$(pwd)":/project   -v "$HOME/.dockagator":/root/.local/share   gatoreducator/dockagator
```

This command will use `"$(pwd)"` (i.e., the current directory) as the project directory and `"$HOME/.dockagator"` as the cached GatorGrader directory. Please note that both of these directories must exist, although only the project directory must contain something. Generally, the project directory should contain the source code and technical writing of this assignment, as provided to a student through GitHub. Additionally, the cache directory should not contain anything other than directories and programs created by DockaGator, thus ensuring that they are not otherwise overwritten during the completion of the assignment.  If the above `docker run` command does not work correctly on the Windows operating system, you may need to instead run the following command to work around limitations in the terminal window:

Windows, putting the command all one line,

```
docker run --rm --name dockagator -v "%cd%:/project" -v "%HomeDrive%%HomePath%/.dockagator:/root/.local/share" gatoreducator/dockagator
```

Please note, these GatorGrader commands have been prepared for you in your ```rDockers/``` directory which should be run in your assignment repository.

## Assistance
To do well on this task, you should also review the chapters of the course textbook and the relevant course slides. Please see the course instructor or one of the Technology Leaders or departmental tutors if you have questions. Finally, you can schedule a meeting during the course instructor's office hours.
