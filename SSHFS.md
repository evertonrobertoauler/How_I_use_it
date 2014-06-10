# SSHFS to sinchronize files

Instalation 

    #Fedora
    sudo yum install fuse-sshfs
    #
    #Debin or Ubuntu
    sudo apt-get install sshfs
    

Sinchronize Folder

    sshfs user@host:/path/to/folder/ /path/to/folder/ -o allow_other -o nonempty
    #
    # or
    #
    sshfs /path/to/folder/ user@host:/path/to/folder/ -o allow_other -o nonempty
    #
    # or
    #
    sshfs user-1@host:/path/to/folder/ user-2@host:/path/to/folder/ -o allow_other -o nonempty
    
Sincronize deactivate

    sudo fusermount -u /path/to/folder/
