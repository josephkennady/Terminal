# How to Run Jupyter Notebook on Ubuntu

This guide covers the steps to install and run Jupyter Notebook on Ubuntu, as well as how to troubleshoot common issues.

## Steps to Install and Run Jupyter Notebook

### 1. Install Python and Pip
Ensure Python and `pip` (Python's package installer) are installed by running the following commands in your terminal:

```bash
python3 --version
pip3 --version

If they aren't installed, you can install them with:

bash
Copy code
sudo apt update
sudo apt install python3 python3-pip
2. Install Jupyter Notebook Using Pip
Install Jupyter Notebook by running:

bash
Copy code
pip3 install jupyter
3. Start Jupyter Notebook
Once installed, you can launch Jupyter Notebook by running:

bash
Copy code
jupyter notebook
This command should open a new tab in your default browser, showing the Jupyter Notebook dashboard. If it doesn't open automatically, you can manually navigate to http://localhost:8888 in your browser.

4. Troubleshooting Tips
If Jupyter Notebook is still not working, check the following:

PATH Issues: Sometimes, Jupyter may not be in your PATH. Try launching it with the full path:

bash
Copy code
~/.local/bin/jupyter notebook
Firewall/Proxy: If you’re using a firewall, ensure it allows access to localhost:8888.

Reinstall Jupyter: In case of broken dependencies, try reinstalling Jupyter:

bash
Copy code
pip3 uninstall jupyter
pip3 install jupyter
Jupyter Lab: As an alternative to Jupyter Notebook, you can use JupyterLab (an updated environment):

bash
Copy code
pip3 install jupyterlab
jupyter-lab
Fixing PATH Issues for Jupyter Notebook
If ~/.local/bin/jupyter notebook works but jupyter notebook does not, you can add ~/.local/bin to your PATH. Here’s how to do it:

Open the Profile File:

For Bash users, open .bashrc in a text editor:

bash
Copy code
nano ~/.bashrc
For Zsh users, open .zshrc:

bash
Copy code
nano ~/.zshrc
Add the Path:

Scroll to the end of the file and add the following line:

bash
Copy code
export PATH="$PATH:$HOME/.local/bin"
Save and Close the File:

In nano, press CTRL + O to save the changes, then press Enter. Press CTRL + X to exit nano.
Apply the Changes:

To make these changes take effect immediately, run this command:

bash
Copy code
source ~/.bashrc  # Or `source ~/.zshrc` for Zsh users
After completing these steps, you should be able to start Jupyter Notebook by simply typing:

bash
Copy code
jupyter notebook
Let us know if you need further clarification or have additional questions!

yaml
Copy code

---

### Instructions for Using This File

1. Copy the entire Markdown content above.
2. Create a new file in your GitHub repository, naming it something like `README.md` or `Jupyter_Notebook_Ubuntu_Guide.md`.
3. Paste the content into the file and save it.

This `.md` file will now be viewable in Markdown format directly on GitHub. Let me know if you have any other requests!
