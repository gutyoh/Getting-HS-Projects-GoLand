# Preface

There currently is a problem with **GoLand** when trying to "get" projects from Stepik, because the projects aren't considered **Go** projects, but **Python** projects.

To overcome this issue you'll need to use **PyCharm** to "get" the project files, and then use **GoLand** to properly run the tests. 

_Take notice that there is another way to only use one IDE to get both the project files and run the tests at the same time. This is done with **IntelliJ IDEA** and having the **Go**, **Python** and **EduTools** plugins installed -- however, this guide won't cover how to use **IntelliJ IDEA** it will cover how to use **PyCharm** and **GoLand**._

# Step #1

Open **PyCharm** (also do not use **PyCharm EAP** versions as it usually has bugs that aren't compatible with `EduTools`) and then go to `Settings->Plugins:`

Search for `EduTools` in the `Marketplace` tab and then install it. Always remember when "getting" project files, to make sure that you have installed the **EduTools** plugin and that it is updated to the latest version:

![pycharm_edutools](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/pycharm_edutools.png?raw=true)


# Step #2

Now, you need to make sure you're logged in to Stepik. To do so, go to `Settings->Tools` then on the left side menu select `Tools->Education`:

![pycharm_settings_tools_education](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/pycharm_settings_tools_education.png?raw=true)

After that just click `Log in to Stepik` and follow the steps to authorize `EduTools` to sync your **PyCharm** IDE with Stepik.

# Step #3

After logging in to Stepik and having `EduTools` installed, Press `Ctrl+Shift+A` Windows/Linux or `Cmd+Shift+A` on macOS and then type `Experimental Features`:

![enable_experimental_features](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/enable_experimental_features.png?raw=true)

# Step #4

Scroll down and enable `edu.course.hyperskill` from the list:

![edu.course.hyperskill](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/select_edu.course.hyperskill.png?raw=true)

# Step #5

Before you can "get" the project files, you'll need to find out the **Stepik Lesson ID** for the project. For example, if you wanted to get the [**University Admission Procedure**](https://hyperskill.org/projects/234) project from the Go track, you would go to the project in the Hyperskill website and then click any of the stage implementations, let's say [Stage #1](https://hyperskill.org/projects/234/stages/1172/implement).

At the bottom of the `Code Editor` of Stage #1 you'll need to click the pencil ✏️ icon to open the project in Stepik:

![pencil_icon](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/pencil_icon.png?raw=true)

Then the Stepik website that holds the project will show up. **Take notice that you'll need _Teacher_ access in Stepik to be able to view/edit project stages!** Finally, you'll be able to see the **Stepik Lesson ID** in the URL:

![lesson_id](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/stepik_project_lesson_id.png?raw=true)

As you can see, the **Stepik Lesson ID** for the **University Admission Procedure** project is `661613`.

# Step #6

Now that you have the **Stepik Lesson ID**, the next step is to once again press `Ctrl+Shift+A` Windows/Linux or `Cmd+Shift+A` on macOS, and then type `Get Hyperskill Lesson from Stepik`:

![get_hyperskill_lesson_from_stepik](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/get_hyperskill_lesson_from_stepik.png?raw=true)

# Step #7

In the `Get Hyperskill Lesson from Stepik` dialogue box you must enter the **Stepik Lesson ID** for the project you wanted to "get" and click `OK`:

![get_lesson_dialogue_box](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/get_lesson_dialogue_box.png?raw=true)

**An important detail is that if you didn't log into Stepik as mentioned in _Step #2_ **PyCharm** won't be able to "get" the project stages/files, and you'll get the following error:**

![failed_to_get_lesson](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/failed_to_get_lesson.png?raw=true)

# Step #8

Finally, if you're properly logged into Stepik after entering the correct lesson ID and clicking `OK`, you'll see the following dialogue box in **PyCharm**:

![get_project_dialogue_box](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/get_project_dialogue_box.png?raw=true)

In the `Title` box you can leave the project title as is: `Hyperskill lesson 661613`, but we recommend naming it as the project name. In this case: `**`University Admission Procedure`**`.

Finally, click the `Create` button, after that all the project files will be loaded into **PyCharm**:

![project_files_loaded_pycharm](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/project_files_loaded_pycharm.png?raw=true)

# Step #9

Now that you have all the project files, you'll need to close **PyCharm**, and open the project in **GoLand**:

![opening_project_files_goland](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/opening_project_files_goland.png?raw=true)

# Step #10

The next step is to make sure you have installed both `EduTools` and `Python Community Edition` plugin in **GoLand**, to do so, go to `Settings->Plugins` and search for them in the `Marketplace` and then install them:

![goland_required_plugins](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/goland_required_plugins.png?raw=true)

# Step #11

Now you'll need to configure a **Python Interpreter** in **GoLand** to be able to run the tests. To do so, go to `Settings->Build, Execution, Deployment` and then click `Python Interpreter`:

![goland_python_interpreter](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/goland_python_interpreter.png?raw=true)

# Step #12

In the **GoLand** Python interpreter selection dialogue box, click the three little vertical dots on the right side, and then click `Add`:

![python_interpreter_selection](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/python_interpreter_selection.png?raw=true)

# Step #13

In the `Add Python Interpreter` dialogue box, click the `Existing environment` radio button and then click the three little vertical dots on the right side:

![add_python_interpreter](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/add_python_interpreter.png?raw=true)

# Step #14

Next, a file explorer dialogue box will show up. Here you must use the file explorer dialogue to navigate to the folder where your project files are:

![file_explorer_selecting_python_interpreter](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/file_explorer_selecting_python_interpreter.png?raw=true)

Since a Python interpreter that has the `hs-tests-python` package is included with the project files you got from Stepik; once you are within the project folder, you'll need to navigate to: `.idea/VirtualEnvironment/Scripts` and then select `python.exe`.

# Step #15

After selecting `python.exe`, the `Add Python Interpreter` dialogue box should look like this, and you would click `OK`:

![selected_python_interpreter](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/selected_python_interpreter.png?raw=true)

# Step #16

You'll be sent back to the `Settings->Build, Execution, Deployment` dialogue box, here you can see that the project python interpreter has both the `hs-test-python` and `psutil` packages which are required to properly run the _tests.py_ files to check the solution for each project stage:

![python_interpreter_packages](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/python_interpreter_packages.png?raw=true)

Finally you can click `Apply` and then `OK` to exit the `Settings->Build, Execution, Deployment` dialogue box. 

# Step #17

Now, you can write a Go reference solution for Stage #1, for example:

![stage1_solution](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/stage1_solution.png?raw=true)

# Step #18

After writing the Go reference solution, right-click the _tests.py_ file for Stage #1 and click `Run` to run the tests:

![run_tests.py](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/run_tests.py.png?raw=true)

If your reference solution is correct all tests will pass, and you'll see the output:

![tests_passed_goland](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/tests_passed_goland.png?raw=true)

# TROUBLESHOOTING COMMON ERRORS

**_A VERY IMPORTANT DETAIL is that for some reason the `hs-test-python` package included in the Project Files has an error, and doesn't properly run the tests._**

**To fix this issue you'll need to do TWO things:**

1. Go to the [`releases` page of the GitHub repository](https://github.com/hyperskill/hs-test-python/releases) for `hs-test-python`. From there, download the `Source code.tar.gz` file for the latest `hs-test-python` release, currently it is `v9`:

![hs-test-python-release](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/hs-test-python-release.png?raw=true)

2. After downloading the _hs-test-python.tar.gz_ latest release, you'll need to go to the `Python Packages` tab at the bottom of **GoLand**_:

![delete_hs-test-python](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/delete_hs-test-python.png?raw=true)

As you can see in the above picture, you'll need to select the `hs-test-python` package and then click the three little vertical dots on the right side, and then click `Delete Package`.

After the old `hs-test-python` package has been deleted, click the `Add Package` button and then click `From Disk`:

![add_package_from_disk](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/add_package_from_disk.png?raw=true)

Next, in the `Install Package` dialogue box, you'll click the small folder 📁 icon and a file explorer window will show up. Here you need to navigate to the folder where you previously downloaded the _hs-test-python.tar.gz_ file:

![add_package_from_disk](https://github.com/gutyoh/Getting-HS-Projects-GoLand/blob/master/blob/select_package_disk.png?raw=true)

After selecting the new release of the _hs_test_python.tar.gz_ file, click `OK` in the file explorer window, and in the `Install Package` dialogue box.

**Finally, the new version of the `hs-test-python` package will now have been installed, and you'll be able to properly run all _tests.py_ file of each project stage! Good job troubleshooting!**
