# learning_python_testing

## Test List:

* [ ] Prototype with Jupiter.
* [ ] Test New [Command Line with Jupyter](https://software.intel.com/en-us/dl-training-tool-devguide-using-jupyter-notebook-terminal-console)
* [ ] Test xterm.js
* [ ] Test codiad
* [ ] Test c9 Ace Install
* [ ] Jupiter test Webcam Examples, running without a command line.


## Install Jupyter

Run the commands I plugged into an install script with `sudo bash install_jupyter.sh`

## Configure the Notebook Server

These were [cherry picked from this page on configuring from a public server.](http://jupyter-notebook.readthedocs.io/en/stable/public_server.html#notebook-public-server)

Create a password manually: `jupyter notebook --generate-config`
Generate a config:  `jupyter notebook --generate-config`

Edit the config file:  `sudo nano /home/pi/.jupyter/jupyter_notebook_config.py`
Fish out the following:
* `c.NotebookApp.ip = '*'`
* `c.NotebookApp.open_browser = False`
* `c.NotebookApp.port = 80`
* `c.NotebookApp.base_url = '/jupyter'` (You can change this to any url you like.)

Other config options to note . . .  you can modify to [embed within another website with this.](http://jupyter-notebook.readthedocs.io/en/stable/public_server.html#embedding-the-notebook-in-another-website)
