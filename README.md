# open-markdown

https://dillinger.io/
可以在线编辑些东西。

https://wiki.qt.io/Qt5_dependencies
Qt5 dependencies
sudo apt-get install build-essential
sudo apt-get install libx11-xcb-dev libglu1-mesa-dev

https://wiki.qt.io/Deploying_a_Qt5_Application_Linux
Creating a standalone application bundle
Deploying a Qt5 application for Linux as a standalone bundle involves bundling it with the necessary Qt components that are needed for the application to run. These can be Qt libraries, Qt plugins, and especially the Qt platform plugin.

A deployment tool is available that automates the prodecures described here and provide an AppImage.
https://github.com/probonopd/linuxdeployqt
http://appimage.org/
If you want one utility for cross platform deploy use a cqtdeployer tool for deploy qt on linux and windows.

Section to be expanded. In the meantime, see http://doc.qt.io/qt-4.8/deployment-x11.html

https://discourse.appimage.org/t/linuxdeployqt-new-linux-deployment-tool-for-qt/57/20

https://github.com/linuxdeploy/linuxdeploy-plugin-qt

https://www.qt.io/blog/deploying-to-linux-with-cmake
Summary
We have seen how to deploy a simple Qt application on Linux using Qt 6.5's CMake deployment API. There's no dedicated linuxdeployqt tool. The current solution wholly relies on CMake's built-in functionality.
These are the platforms that are covered by Qt's CMake deployment API:
Windows
macOS
Linux
For Android and iOS there's still the need to call androiddeployqt / macdeployqt manually - or you let Qt Creator handle these details.

https://doc.qt.io/qt-6/deployment.html
https://doc.qt.io/qt-6/linux-deployment.html

https://ubuntu.com/blog/how-to-create-snap-packages-on-qt-applications

https://doc.qt.io/qt-6/integrity-installing-dependencies.html

结论：
3种方法：
1. linuxdeployqt
2. cmake
	Qt6 才有的功能？
3. snap
	还需要在目标系统上安装 snap。