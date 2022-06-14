# NevisROOTtutorialAtTufts

Just some quick notes and materials when completing the Nevis ROOT tutorial on Tufts

# Accessing Meitner

I've setup a computer that has ROOT and jupyter notebooks that sould let you run the tutorial.

To use it, first request a user name from me.

To log in, you need to be connected to the Tufts VPN.

Once connected to the VPN, you can ssh into the machine using:

     ssh -XY -L 8005:localhost:8005 [username]@130.64.84.151

Note the '8005' used above. This the port we can use to give us access to the jupter notebook.

If you see a message along the lines of "This port is already in use", log out of the ssh connection by typing `exit` and run the command again with a different port number (80XX).

# Setting up up ROOT

Run:

    source /usr/local/bin/thisroot.sh


This will setup some environment variables that are needed for PyROOT.

# Starting a jupyter notbook

Note: you need to first setup ROOT before running the following command to start a notebook.

     jupyter-notebook --no-browser --port=8005


Make sure the port matches the one used above. You'll see some instructions for copy and pasting a url. Do so in your machine's (e.g. the laptop you're using) web browser.

If it doens't work, you might see a message about the port being in use. Re-log into the computer with a new port number and try again.
     