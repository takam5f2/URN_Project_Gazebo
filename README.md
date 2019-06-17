# Robotics Nanodegree Project 1: Gazebo Excersize

### Summary of the repository
Here, I located some files for gazebo configuration.
These files are evaluated on udacity Robotics software nanodegree.

I followed [Project Rubrics](https://review.udacity.com/#!/rubrics/2346/view).


I created the following required objects:

* Building

Here I designed the building whose structure resembles that of my house.
The building is located on `model/myhouse/` directory.

* Model Objects

I created box cart here. The model is located on `model/mymodel_cart` directory.
 
* Script

I wrote very simple script which prints "Welcome to Takayuki's World!" on terminal.
The script is located on 'script' directory

* World

World file contains the building and some models.
If you open the world with gazebo command, the message defined in the script will be printed out on your terminal.


### Execution

#### Git clone and Compile
Before opening the file, you have to compile gazebo script file.

You have to follow the command line as below.

```
$ pwd
/home/<user_name>/work       // sample execution result

$ git clone https://github.com/takam5f2/URN_Project_Gazebo.git
// you can find the files which are donwloaded from this repository.

$ mkdir build
$ cd build

$ cmake ../
$ make

// The script file must be compiled
```

After executing the commands above, you can find the file named `libwelcome_message.so` file.

Please execute the next command which indicates the path including `libwelcome_message.so`

```
$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/<user_name>/work/URN_Project_Gazebo/build
```

If you executed commands shown above without any error, you can execute gazebo.

### Execution
You only have to execute gazebo command in order to confirm my achievement.

```
$ pwd

/home/<user_name>/work/URN_Project_Gazebo/build
 
$ cd ../world

$ gazebo myproj_myhouse.world
Welcome to Takayuki's world!
```

You can see what my world is designed with my building and cart model.




EOF
