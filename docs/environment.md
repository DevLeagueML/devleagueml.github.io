# Setup your Environment & Register for the Competition

## Requirements
- Unix / Linux (recommended)
- Python3.9+
- gcc / g++ version 9+


## Installation

- Check python version and make sure it is `3.9` or above, otherwise go to [Python](https://python.org) to download a more recent version of Python.

    ```bash
    python3 --version
    ```

- Create a root directory for your competition work and navigate to the new directory. A good name for this directory is `devleague`.

    === "Linux"

        ```bash
        mkdir ~/<devleague_root> && cd ~/<devleague_root>
        ```
        
    === "Windows"

        ```batch
        mkdir C:\Users\<username>\<devleague_root> && cd C:\Users\<username>\<devleague_root>
        ```

### Virtual Environment Installation (Recommended)

- Move to your newly created directory if you are not already and create a virtualenv environment

    === "Linux"

        ```bash
        cd ~/<devleague_root>
        ```

        ```bash
        python3 -m venv .
        ```

    === "Windows"

        ```batch
        cd C:\Users\<username>\<devleague_root>
        ```

        ```batch
        python3 -m venv .
        ```

- Make sure you are in your `<devleague_root>` directory. Or make sure you reference the right path to the directory.

- Activate environment

    === "Linux"

        ```bash
        source ~/<devleague_root>/bin/activate
        ```

    === "Windows"

        ```batch
        <devleague_root>\Scripts\activate.bat
        ```

- Get to the root directory if you are not already there
   
    === "Linux"

        ```bash
        (venv) cd ~/<devleague_root>
        ```

    === "Windows"

        ```batch
        (venv) cd C:\Users\<username>\<devleague_root>
        ```
    
- Install walancli

    === "Linux"

        ```bash
        (venv) $ pip install -U https://github.com/s7d11/walancli/0.0.1v/walancli.tar.gz
        ```

    === "Windows"

        ```batch
        (venv) C:\> python -m pip install -U https://github.com/s7d11/walancli/0.0.1v/walancli.tar.gz
        ```

- Note that you can deactivate the environment with `#!sh (venv) $ deactivate`.

### System Intallation

- Install walancli


    ```bash
    python3 -m pip install -U https://github.com/s7d11/walancli/0.0.1v/walancli.tar.gz
    ```

### Verify installation


```bash
walan --version
```

You should see the following as output

```
(C) 2022 WalanSO

Version=0.0.1-pre_alpha
```

* If you encounter an issue while installing, reach out to us [Email]('sdiarra@robotsmali.org')

## Registration / Authentication

- Run the following command to perform authentication

    ```bash
    walan auth
    ```

- Proceed to entering your personal details to complete authentification.

- Select register if you do not have an account already

    ```bash
    ? I would like to: 
    login
    ❯ register
    ```

- Select `student` here

    ```
    ? I would like to: register
    ? Are you a: 
    proctor
    ❯ student
    ```

- Proceed to fill out your credentials accordingly, assure to have a valid email account.

    ```bash
    ? I would like to: register
    ? Are you a: student
    ? Enter your fullname: Amadou Ahmed
    ? Enter your email: aahmed@email.com
    ? Are you an active student? No
    ? Enter password: 
    ? Confirm password: ****
    ? Proceed with registration? (y/N)
    ```

- Once you confirm you see a message saying you `Successfully register to WalanSO`

- Run the following command to verify your authentification.

    ```bash
    walan whoami
    ```

- Congratulations you are all set for the competition, keep checking here you might find something cool here for you.

<!--
## Test your skills

- Pull challenge file. Make sure you are in the devleague `<root>` directory.

```bash
walan devlg dl001 get defi0 && cd defi0
```

- You are ready for the challenge now.
-->
