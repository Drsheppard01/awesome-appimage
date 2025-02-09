<!--lint disable double-link-->

<div align="center">
	<div>
		<img width="500" src="media/logo.svg" alt="Awesome AppImage">
	</div>
	<a href="https://awesome.re">
		<!img src="https://awesome.re/badge-flat2.svg" alt="Awesome">
	</a>
	<p>
		<sub>Lovingly crafted AppImage tools and resources. Follow me on <a href="https://twitter.com/probonopd">Twitter</a>.</sub>
	</p>
	<br>
</div>

# Awesome AppImage [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[AppImage](https://appimage.org) is a community-based format to distribute applications to various mainstream Linux distributions without the need for a centralized store. One app = one file! This list contains tools to work with AppImages, such as to create AppImages for applications and to integrate AppImages into the system easily. As the vibrant community around AppImage is growing, so is this list.

## Contents

- [AppImage discovery](#appimage-discovery)
	- [App catalogs](#app-catalogs)
	- [App stores](#app-stores)
	- [App centers](#app-centers)
- [AppImage consumption tools](#appimage-consumption-tools)
	- [Desktop integration](#desktop-integration)
	- [Updaters](#updaters)
	- [Sandboxes](#sandboxes)
	- [Package managers](#package-managers)
	- [Linux distributions](#linux-distributions)
- [AppImage developer tools](#appimage-developer-tools)
	- [Low-level tools](#low-level-tools)
	- [Build systems](#build-systems)
	- [Deployment tools for compiled applications](#deployment-tools-for-compiled-applications)
	- [Deployment tools for Python applications](#deployment-tools-for-python-applications)
	- [Deployment tools for Electron applications](#deployment-tools-for-electron-applications)
	- [Deployment tools for Java applications](#deployment-tools-for-java-applications)
	- [Deployment tools for .NET Core (Mono) applications](#deployment-tools-for-net-core-mono-applications)
	- [Deployment tools for Rust applications](#deployment-tools-for-rust-applications)
	- [Tools to convert from other package formats](#tools-to-convert-from-other-package-formats)
	- [Metadata tools](#metadata-tools)
	- [QC tools](#qc-tools)
	- [Continuous integration](#continuous-integration)
	- [Libraries](#libraries)
	- [Templates](#templates)
- [Resources](#resources)
	- [Specs](#specs)
	- [Documentation](#documentation)
	- [Tutorials](#tutorials)
	- [Articles](#articles)
	- [Videos](#videos)
	- [Books](#books)
	- [Blogs](#blogs)
	- [Courses](#courses)
	- [Community](#community)
	- [Miscellaneous](#miscellaneous)
	- [Related](#related)
	- [Other awesome lists](#other-awesome-lists)

## AppImage discovery

### App catalogs

- [AppImage.GitHub.io](https://appimage.github.io/) - Catalog of AppImages that passed an automated test, links to upstream download pages.
- [Apps For Linux](https://apps-for-linux.github.io/) - Simple application catalog oriented on active development apps
- [Get AppImage](https://g.srev.in/get-appimage/) - Collection of all AppImages in one website. Great search functionality.
- [PORTABLE LINUX APPS](https://portable-linux-apps.github.io/) - AppImage catalog specially developed for AM

### App stores

- [AppImageHub.com](https://www.appimagehub.com/) - Downloadable AppImages, powered by [Opendesktop.org](https://www.opendesktop.org/).

### App centers

- [NX Software Center](https://github.com/Nitrux/nx-software-center) - Portable Software Center for portable AppImage applications.

## AppImage consumption tools

### Desktop integration

- [app-hub](https://github.com/cosmic-utils/app-hub) - AppHub is a Linux desktop application that simplifies the installation and management of .appImage packages
- [appimage-desktop-integrator](https://github.com/8ByteSword/appimage-desktop-integrator) - This bash script automates the process of creating desktop entries with icons for AppImage applications. 
- [appimage-integrator](https://github.com/apapamarkou/appimage-integrator) - With this tool, you can easily add or remove AppImage applications from your system's application menus and launchers
- [AppImageLauncher](https://github.com/TheAssassin/AppImageLauncher) - Integrates into users' systems and establishes a single `~/Applications` directory, assisting the user to move AppImages into there, with support for updating and removing AppImages through apps launcher.
- [Gear lever](https://github.com/mijorus/gearlever/) - Integrates AppImages into the Gnome desktop by drag-and-drop onto the Gear lever application.
- [go-appimaged](https://github.com/probonopd/go-appimage/tree/master/src/appimaged) - Optional daemon that integrates AppImages into the system (experimental).
- [install-appimage](https://github.com/bl4ckj4ck777/install-appimage) - Install AppImage files like regular applications on Ubuntu 24.04
- [LinuxPA](https://github.com/CalebQ42/LinuxPA) - PortableApps.com type launcher for Linux with AppImage support.
- [XApp Thumbnailers](https://github.com/linuxmint/xapp-thumbnailers) - Thumbnailers for GTK Desktop Environments, including one for the AppImage file format. Makes Gtk based file managers like Caja (MATE), Nautilus (GNOME), Nemo (Cinnamon), PCManFM (LXDE), and Thunar (Xfce) show application icons on AppImages.

### Updaters

- [AppImageUpdate](https://github.com/AppImageCommunity/AppImageUpdate) - Official grapical application to update AppImages; command-line tool to update AppImages.

### Sandboxes

- [AppImage Sandboxing Project](https://github.com/mgord9518/aisap) - Golang library to help sandbox AppImages with bwrap.
- [Firejail](https://github.com/netblue30/firejail) - Optional sandbox with support for AppImage built in.

### Package managers

__Note:__ The AppImage format is explicitly designed _not to need any package managers_ or similar tools. Everything can be done in the file manager (and an optional daemon for system integration).

- [AppMan](https://github.com/ivan-hc/AppMan) - AppImage Manager that works like APT or Pacman.
- [bauh](https://github.com/vinifmor/bauh) - Graphical user interface for managing Linux applications supporting AppImage, Arch (repositories/AUR), Flatpak, Snap and native Web applications.
- [pho](https://github.com/zyrouge/pho) - The AppImage Manager that Linux always deserved.

### Linux distributions

Although the AppImage format was carefully designed not to need any special support from Linux distributions, there are some that offer varying degrees of AppImage friendliness out of the box.

- [Deepin](https://www.deepin.org/en/) - When you double-click an AppImage or any other executable file that lacks execute permissions, a user-friendly dialog explains the situation and asks for your permission to set the execute permission and execute the executable.
- [Linux Mint](https://linuxmint.com/) - Has an [AppImage thumbnailer](https://github.com/linuxmint/xapp-thumbnailers) to show application icons on AppImage files.
- [Nitrux](https://nxos.org/) - Promotes the use of AppImage as the main format for getting applications, has a built in app center featuring AppImages.
- [Zenwalk GNU Linux](http://www.zenwalk.org/) - Is "AppImage ready" and distributes some applications in AppImage format.

## AppImage developer tools

### Low-level tools

- [appimageutils](https://github.com/leleliu008/appimageutil) - A command-line utility to generate AppImage. Written in Shell
- [appimagetool](https://github.com/AppImage/AppImageKit/releases/tag/continuous) - Converts AppDirs into AppImages.
- [nix-bundle](https://github.com/matthewbauer/nix-bundle) - Converts Nix derivations into AppImages.

### Build systems

- [appimagecraft](https://github.com/TheAssassin/appimagecraft) - Recipe based AppImage creation tool working from source.
- [KDE Craft](https://invent.kde.org/packaging/craft) - Build system used by KDE that can produce AppImages and other formats.
- [AppImage.cmake](https://github.com/Ravbug/AppImage.cmake) - CMake script which facilitates generating AppImage executables for Linux.
- [rules_appimage](https://github.com/lalten/rules_appimage) - Bazel rules to package any lang_binary target as AppImage.

### Deployment tools for compiled applications

- [appimagetool](https://github.com/AppImage/appimagetool/) - Reference implementation appimagetool - utility which use to convert AppImage from AppDirs
- [go-appimagetool](https://github.com/probonopd/go-appimage/tree/master/src/appimagetool) - Tool that deploys dependencies into AppDirs, and converts AppDirs into AppImages (experimental).
- [linuxdeployqt](https://github.com/probonopd/linuxdeployqt) - Deploys dependencies into AppDirs and creates AppImages; for Qt and other compiled applications.
- [linuxdeploy](https://github.com/linuxdeploy/linuxdeploy) - AppDir creation and maintenance tool using plugins.
- [XojoToAppImage](https://github.com/AlwaysOfflineSoftware/XojoToAppImage) - Graphical tool for packaging compiled Xojo Linux programs into AppImages.

### Deployment tools for Python applications

- [Briefcase](https://briefcase.readthedocs.io/) - Convert Python project into a standalone native application, e.g., using AppImage.
- [linuxdeploy-plugin-conda](https://github.com/linuxdeploy/linuxdeploy-plugin-conda) - Bundle Python into an AppDir using a source distribution, Conda, and linuxdeploy.
- [pyproject-appimage](https://codeberg.org/JakobDev/pyproject-appimage) - pyproject-appimage allows you to create a AppImage in a few seconds.
- [python-appimage](https://github.com/niess/python-appimage) - Ready to use AppImage distributions of Python (can be modified to include your application).

### Deployment tools for Electron applications

- [electron-builder](https://github.com/electron-userland/electron-builder) - Supports AppImage as an output format.
- [ReForged-maker-appimage](https://github.com/SpacingBat3/ReForged/tree/master/makers/appimage) - An unofficial AppImage target maker for the Electron Forge

### Deployment tools for Haskell applications

- [cabal-appimage](https://github.com/gbrsales/cabal-appimage) - This package provides a build hook for Cabal automating the creation of AppImage bundles.

### Deployment tools for Java applications

- [script from Cryptomator](https://github.com/cryptomator/cryptomator/blob/develop/dist/linux/appimage/build.sh) - publish AppImage with JavaFX


### Deployment tools for .NET Core (Mono) applications

- [DotnetPackaging](https://github.com/SuperJMN/DotnetPackaging) - Tool to distribute .NET applications in the AppImage format.
- [PupNet Deploy](https://github.com/kuiperzone/PupNet-Deploy) - Cross-platform deployment utility which publishes your .NET project and packages it as a ready-to-ship installation file in a single step.
- [.NET Core AppImage example](https://github.com/ppy/osu-deploy/blob/697a49e9602502a2b7a899c0dff5383f6512d5d2/Program.cs#L207-L243) - Example of how to deploy .NET Core (Mono) applications as an AppImage using `dotnet publish -f netcoreapp3.1 -r linux-x64` from within a `.cs` program.

### Deployment tools for Rust applications


### Tools to convert from other package formats

- [AppImaGen](https://github.com/ivan-hc/AppImaGen) - Generates an AppImage from Debian or from a PPA of your choice for the previous (unfortunately not the oldest as recommended) and still supported Ubuntu LTS.
- [appimage-bash](https://github.com/valicm/appimage-bash) - GitHub Action for creating AppImage releases from binaries inside `.tar.gz` archives.
- [GMAppImager](https://github.com/time-killer-games/GMAppImager) - Graphically Converts GameMaker Studio 2 games to AppImage bundles.
- [pkg2appimage](https://github.com/AppImage/pkg2appimage) - Converts from deb, zip, tar.gz and other formats to AppImage using YAML recipes.
- [snap2appimage](https://github.com/ivan-hc/Snap2AppImage) - An experimental script to convert Snap packages to portable AppImages

### Metadata tools

- [AppStream MetaInfo Creator](https://www.freedesktop.org/software/appstream/metainfocreator/#/) - More elaborate generator for AppStream MetaInfo files by the author of the AppStream metainfo format.

### QC tools

- [appimagelint](https://github.com/TheAssassin/appimagelint) - Tool to check AppImages for compatibility, best practices etc.

### Continuous integration

- [GitHub Actions example](https://github.com/probonopd/Zoom.AppImage/blob/master/.github/workflows/main.yml) - Example of how to upload AppImages built using GitHub Actions to GitHub Releases.
- [build-appimage-action](https://github.com/AppImageCrafters/build-appimage-action) - GitHub Action for producing AppImages using appimage-builder.
- [jniltinho/packages](https://github.com/jniltinho/packages) - Drone.io example for producing AppImages using go-appimagetool.
- [Link to the latest build artifact on GitLab CI](https://gitlab.com/linuxappimage/element-desktop/-/jobs/artifacts/master/raw/Element.AppImage?job=run-build) - Example of how to directly link to the latest build artifact on GitLab CI (can be tricky).

### Libraries

- [appenv](https://github.com/TheMarlboroMan/appenv) - Small C++ library telling where the app data resides and where the user data is by using `readlink("/proc/self/exe")`), thus allowing C++ applications to become relocatable in the filesystem.
- [libappimage](https://github.com/AppImage/libappimage) - Implements functionality for dealing with AppImage files, written in C++ using Boost.

### Templates

- [Briefcase Linux AppImage Template](https://github.com/beeware/briefcase-linux-appimage-template) - Cookiecutter template for building Python apps that will run under Linux, packaged as an AppImage.
- [mini-qml](https://github.com/patrickelectric/mini-qml) - Minimal Qml application template with deployment for Linux (AppImage), Windows, macOS and WebAssembly.
- [Qt Desktop Template](https://github.com/stemoretti/qt-desktop-template) - Template for creating Qt Widgets desktop applications with AppImage generation using linuxdeployqt.
- [qt-hello-world](https://github.com/AppImageCrafters/qt-hello-world) - Qt Hello World project for AppImage creation using appimage-builder.
- [qt-qml-project-template-with-ci](https://github.com/219-design/qt-qml-project-template-with-ci) - Template for a Qt/QML application with batteries included: GitHub CI, automated GUI testing, automatic code-format checks and more. Compiles for Linux (AppImage), Mac, and Android.
- [wxWidgetsTemplate](https://github.com/Ravbug/wxWidgetsTemplate) - Cross-platform application template for wxWidgets C++, with pre-set files and IDE projects, supporting AppImage.

## Resources

### Specs

- [AppImageSpec](https://github.com/AppImage/AppImageSpec) - Official specification for the AppImage format.
- [Desktop Entry Specification](https://specifications.freedesktop.org/desktop-entry-spec/latest/) - Specification for the matadata used inside AppImages.

### Documentation

- [docs.appimage.org](https://docs.appimage.org/) - Official AppImage documentation.

### Tutorials

- [Produce an AppImage that bundles everything with go-appimage](https://www.youtube.com/watch?v=XTGn_JqmDu0) - How to make an AppImage that bundles _all_ required libraries so that it should run not only on newer, but also on _older_ systems than the build system.

### Articles
- [Getting Started Managing Software with AppImage on Ubuntu](https://adamtheautomator.com/appimage-ubuntu/) - Verbosely explains how to manage AppImages without the need for further software.
- [The Background Story of AppImage](https://itsfoss.com/appimage-interview/) - Interview with the creator of AppImage, explaining the key ideas and motivations behind the concept.
- [Flatpak, Snap and AppImage](https://distrowatch.com/weekly.php?issue=20160704#opinion) - Jesse Smith on DistroWatch about AppImage, Flatpak and Snap.
- [Don't Install, Just Copy with klik](https://dot.kde.org/2005/09/16/dont-install-just-copy-klik) - Article from 2005 that gives perspective on how AppImage started, relevant only for historical reasons now.

### Videos

- [AppImage system integration on Ubuntu using go-appimaged](https://www.youtube.com/watch?v=L00UjifUEfE) - New appimaged daemon from the go-appimage implementation.
- [AppImage: Portable applications for Linux](https://www.youtube.com/watch?v=nzZ6Ikc7juw) - Official AppImage introduction video by its founder.
- [AppImage: Universal Linux Apps, Overview and Thoughts](https://www.youtube.com/watch?v=tMqES2pNxYY) - By Jeremy "Jay" LaCroix, LearnLinuxTV.
- [Comparing Linux Package Formats - Deb, Flatpak, AppImage, etc.](https://www.youtube.com/watch?v=7fPShv-8Z_4) - By Bryan Lunduke.
- [Integrate and Manage AppImages with AppImageLauncher](https://www.youtube.com/watch?v=D2WA2zdLvVk) - By Eric Adams.

### Books

- [Mastering Qt 5](https://www.amazon.de/Mastering-Qt-stunning-cross-platform-applications-ebook/dp/B07DH9YK9Q/) - Contains a section on how to package and deploy Qt applications for Linux using linuxdeployqt.

### Blogs

- [AppImage Crafters Blog](https://appimagecrafters.github.io/) - Blog about AppImage creation an usage by azubieta.
- [AppImage Discussions](https://github.com/orgs/AppImage/discussions) - Github Discussions where you can share your Ideas and engage with the community
- [Planet AppImage](https://appimage.gitlab.io/planet/) - Blog Aggregator covering all things AppImage.
- [TheAssassin Blog](https://assassinate-you.net/tags/appimage/) - Blog covering AppImage related topics by TheAssassin.

### Courses

### Community

- [discourse.appimage.org](https://discourse.appimage.org/) - Official AppImage forum for users and application developers.
- [r/AppImage/](https://www.reddit.com/r/AppImage/) - AppImage subreddit.
- [Stack Overflow](https://stackoverflow.com/tags/AppImage) - Questions tagged `[appimage]` on Stack Overflow.
- [#AppImage channel on libera.chat](https://web.libera.chat/#AppImage) - Chat where AppImage developers and users hang out, be prepared to stay in the channel for days if you don't get answers immediately.

### Miscellaneous

- [AppImage wiki](https://github.com/AppImage/AppImageKit/wiki) - Official AppImage wiki.
- [AppImageZip](https://github.com/sagebind/appimagezip) - Experimental pure Rust implementation of the AppImage runtime that uses Zip as the backing file system image.
- [help-wanted](https://github.com/search?q=user%3Aappimage+label%3Ahelp-wanted+state%3Aopen&type=Issues) - AppImage issues that the AppImage team would like your help with. A great way to get started contributing to the project.

### Related

- [appdwarf](https://github.com/Phantop/appdwarf) - A tool to convert an AppDir or an existing AppImage file, either as a local file or from a URL, into a highly compressed portable image using dwarfs.
- [shImg](https://github.com/mgord9518/shappimage) - An AppImage implementation made in shell script
- [sharun](https://github.com/VHSgunzo/sharun) - Run dynamically linked ELF binaries everywhere (musl and glibc are supported).
- [uruntime](https://github.com/VHSgunzo/uruntime) - Universal RunImage and AppImage runtime with SquashFS and DwarFS supports

### Other awesome lists

- [awesome-linuxdeploy](https://github.com/linuxdeploy/awesome-linuxdeploy) - Awesome list on linuxdeploy.
- [All Awesome Lists](https://github.com/topics/awesome) - All the Awesome lists on GitHub.
