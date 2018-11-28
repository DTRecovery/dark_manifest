# DTRecovery Project

## Getting Started ##
---------------

To get started with OMNI sources to build DTRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

To initialize your local repository using the OMNIROM trees to build DTRP, use a command like this:

```
    repo init -u git://github.com/DTRecovery/dark_manifest.git -b recovery
````   
   
To initialize a shallow clone, which will save even more space, use a command like this:

```
    repo init --depth=1 -u git://github.com/DTRecovery/dark_manifest.git -b recovery
```

Then to sync up:

```
    repo sync
```

Choose build type before start building
```
   $ . build/build.sh
   $ reltypea (FOR OFFICIAL BUILDS)
   $ reltypeb (FOR UNOFFICIAL BUILDS)
   $ reltypec (FOR BETA BUILDS)
```

Then to build:
```

   $  . build/build.sh; lunch omni_<device>-eng; darkify
```
