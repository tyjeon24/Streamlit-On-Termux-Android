# Streamlit-On-Termux-Android

## Project Description
* This project addresses the issue encountered when attempting to install Streamlit in Termux on Android devices.
* Simply typing `pip install streamlit` in Termux does not suffice due to specific dependencies required by Termux Python.


## How to install
1. **Install Termux**
   * Begin by installing the Termux application on your Android device.
2. **Install Streamlit**
    ```bash
    pkg upgrade -y
    pkg install -y tur-repo
    pkg install -y python rust llvm binutils-is-llvm libzmq libjpeg-turbo
    pkg install -y python-numpy python-pandas python-pyarrow
    pip install streamlit
    ```
3. **Resolve Repository Errors**
   * If encountering repository errors in Termux, manually set the repository by executing code below.
    ```bash
    termux-change-repo
    ```
4. **Test Streamlit Installation**
    ```bash
    streamlit hello
    ```

## References
- [Python - Termux Wiki](https://wiki.termux.com/wiki/Python)
- Inspired by [Selenium-On-Termux-Android](https://github.com/luanon404/Selenium-On-Termux-Android) project.