Title:   Workshop preparations
Summary: Session 0: Prerequisites and installation instructions
Authors: Adina Wagner
Date:    2020

# Software installation

If you want to work on your own machine during the workshop, please make sure to install the relevant software in advance.
At the end of this page, a short script can help you to verify that everything works as it should.
If you run into problems, please get in touch **prior** to the workshop.
We are happy to help with installation problems or general questions any time, but have limited time during concurrent teaching in a virtual workshop setting.
Reach out to us about problems as early as you can by filing an issue on our GitHub repository: [github.com/adswa/dl-workshop](https://github.com/adswa/dl-workshop/issues/new).

If you haven't set up the software, you can log into a Jupyter Hub instance we will provide.

| **NOTE FOR WINDOWS USERS** |
|------------------------------------------------------------------|
| DataLad and its underlying tools work less well on Windows. An honest assessment can be found in the [DataLad handbook](http://handbook.datalad.org/en/latest/intro/windows.html). Alternatively to using your Windows OS you can use the Windows Subsystem for Linux (2), your institutions high-performance compute cluster, or the provided Jupyter hub.|

| **NOTE FOR HCP/HTC USERS** |
|------------------------------------------------------------------|
| If you want to use shared high-performance or high-throughput infrastructure, but there is no DataLad installation yet, you can either install the required software on a per-user basis (no root privileges required) following [these instructions](http://handbook.datalad.org/en/latest/intro/installation.html#linux-machines-with-no-root-access-e-g-hpc-systems) in the DataLad Handbook, or you can ask your system's administrator to install the software. Feel free to share adina.wagner@t-online.de as a point of contact for additional information and [handbook.datalad.org/r.html?install](http://handbook.datalad.org/en/latest/intro/installation.html#install) for installation instructions.|


| **The following software is required to follow along interactively.** Please install it as early as you can |
|------------------------------------------------------------------|
| **DataLad**: [handbook.datalad.org/intro/installation.html](http://handbook.datalad.org/en/latest/intro/installation.html) (depending on installation method and operating system, Git and git-annex can already be included a DataLad installation)|
| **Git**: [git-scm.com](https://git-scm.com/)     |
| **git-annex**: [git-annex.branchable.com/](https://git-annex.branchable.com/) |


# An intro to the command line

During the workshop we will primarily work with the command line.
If you are using your own computer, but are not used to typing in your computer's terminal, we recommend that you familiarize yourself with the basics.
You can find a short tutorial [here](http://handbook.datalad.org/en/latest/intro/howto.html).



# Check your installation

To check whether everything worked out, please run the following command in your terminal (without the leading ``$``):

```
$ datalad -f'{infos[git-annex][version]}' wtf
8.20200330
```

If this returns a version number as above (it does not need to be identical to ``8.20200330``), you're good! 👍

### Potential errors:

If you see the following, your Git identity isn't configured yet:

```
It is highly recommended to configure Git before using DataLad. Set both 'user.name' and 'user.email' configuration variables.
```

If you don't get a version number of `N/A`, git-annex is missing. Please double check by typing ``git-annex`` into your terminal and pressing enter - if your shell responds with ``command not found``, please [install git-annex](https://git-annex.branchable.com/install/).

If your shell returns ``command not found``, DataLad is missing. Please double check by retrying this operation in a new shell or typing ``rehash`` beforehand.

# Getting help

If you run into problems, please reach out as early as you can by filing an issue on our GitHub repository: [github.com/adswa/dl-workshop/](https://github.com/adswa/dl-workshop/issues/new).
