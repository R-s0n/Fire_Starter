# Fire Starter

This tool is designed to automate the inital phase of my Recon methodology for Bug Bounty hunting.  
I have specifically designed this script around my workflow, but feel free to take the code and make 
it your own (I love Forks!).  Although I've configured the data structures and requests to work with 
my WAPT Framework, which uses a MongoDB database to store data through a Node/Express API, the code
could be easily refactored to work with a SQL or PostGRES database.  I'll work on a more universally
applicable version of this script as I get closer to releasing my WAPT Framework publically.  -rs0n

******************************************************************************************************
    I AM NOT RESPONSABLE FOR HOW YOU USE THIS TOOL.  DON'T BE A DICK!                     
******************************************************************************************************

    python3 fire_starter.py [-h --help] [-d --domain] [-s --server] [-p --port]
------------------------------------------------------------------------------------------------------
|  Short  |    Long    |  Required  |                               Notes                             |
|---------|------------|------------|-----------------------------------------------------------------|
|   -h    |  --help    |     no     |                   Display this help message                     |
|   -d    |  --org     |     yes    |                   Name of the root/seed FQDN                    |
|   -s    |  --server  |     yes    |           IP Address of the Node server hosting DB API          |
|   -p    |  --port    |     yes    |                Port of Node server hosting DB API               |
-------------------------------------------------------------------------------------------------------

## To Do
1. Pipe all stderr msgs to static log file
2. Add modules for building/scanning with custom wordlists
3. Add EyeWitness module
