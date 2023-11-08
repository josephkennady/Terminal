Sure, here are the steps to create a virtual environment in Ubuntu for Python3:

1. First, you need to install the `python3-venv` package. Open a terminal and run the following command:
```bash
sudo apt-get install python3-venv
```
2. Once the package is installed, you can create a virtual environment using the following command. Replace `myenv` with the name you want to give to your virtual environment:
```bash
python3 -m venv myenv
```
3. After the virtual environment is created, you can activate it using the following command:
```bash
source myenv/bin/activate
```
4. Now your terminal prompt should change to show the name of the activated virtual environment. At this point, you're using the Python and Pip binaries associated with the virtual environment. When you're done with your work, you can deactivate the virtual environment by simply typing:
```bash
deactivate
```
Remember, you need to activate the virtual environment in each terminal where you want to use it. Enjoy coding! 😊
