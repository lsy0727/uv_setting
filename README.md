# uv_setting

## Add the Python installation path

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/5744c020-eea7-4435-acf5-cdf695a98403" />

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/1a81911c-bac8-41d3-aa05-14bcd05dd68c" />

```
# Locate the installation path manually and add it to the PATH
C:\Users\<user name>\AppData\Local\Programs\Python\Python<version>\
C:\Users\<user name>\AppData\Local\Programs\Python\Python<version>\Scripts\
```

-> The pip command is available in PowerShell

## uv install

```
# Open PowerShell and install uv
pip install uv
```

## Add the uv installation path

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/5744c020-eea7-4435-acf5-cdf695a98403" />

<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/6fd2d750-795e-47cd-86c7-9c78d5d23dd1" />

```
# Locate the installation path manually and add it to the PATH
C:\Users\<user name>\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.13_qbz5n2kfra8p0\LocalCache\local-packages\Python<version>\Scripts
```

-> After setting the UV environment variables, you may still be unable to run the <virtual_env_name>/Scripts/activate.ps1 file because of the script execution policy
```
# 1. Run PowerShell as Administrator

# 2. Check the execution policy
# -> You’ll typically see one of the following: Restricted, RemoteSigned, or AllSigned. If it's set to Restricted, you may run into issues.
Get-ExecutionPolicy

# 3. Change the execution policy
Set-ExecutionPolicy RemoteSigned

# The execution policy is for system security, so if you want to revert it back to its original state after use, you can run the following command
Set-ExecutionPolicy Restricted
```
