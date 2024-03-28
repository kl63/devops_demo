# Key Commands:

## Docker Commands & Process

1. **Create Project Folder:**
    ``` sh
    mkdir devops_demo
    cd devops_demo
    ```
<b><i>Create the files needed in project</i></b>

2. **Create & Activate Virtual Env.:**
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```
3. **Installing Packages:**
    ```sh 
    touch requirements.txt
    pip install <package_name>
    pip freeze > requirements.txt
    ```
4. **Running Pytest (Local):**
    ```sh
    pytest
    ```

5. **Building Docker:**
    ```sh
    docker build -t <image_name> .
    docker run <image_name>
    ```

6. **Running Pytest (Docker):**
    ```sh
    docker run <image_name> -m pytest
    ```

7. **Pushing to Docker:**
1. Create Docker repository on https://hub.docker.com/ 
    ```sh 
    docker build -t <docker_username>/<repository_name> .
    docker push <docker_username>/<repository_name>
    ```

8. **Github Secrets:**
- Located in Github repository
    - Settings > Environments > Environment secrets

9. **Docker Tokens:**
- Located in Docker account 
    - My Profile > Edit profile > Security > New Access Token


## Command Line Commands:

1. **Installation:**
    ```sh
    pip3 install virtualenv
    ```

2. **Activating Virtual Environment:**
    ```sh
    source venv/bin/activate
    ```

3. **Installing Dependencies:**
    ```sh
    pip3 install -r requirements.txt
    ```

4. **Updating Requirements File:**
    ```sh
    pip3 freeze > requirements.txt
    ```

## Testing Commands:

- Run tests without pylint or coverage:
    ```sh
    pytest
    ```

- Run tests with pylint static code analysis:
    ```sh
    pytest --pylint
    ```

- Run tests, pylint, and coverage to ensure all code is tested:
    ```sh
    pytest --pylint --cov
    ```

- Run tests with a specified number of records (e.g., 10):
    ```sh
    pytest --num_records=10
    ```

## Closing Repositories and Setting Up Your Own:

If you have cloned a repository for this project and want to set it up in your own repository, follow these steps:

1. Clone the repository you want to take as your starting point (replace `Cloning Repo URL` with the URL of repository you want to clone):
    ```sh
    git clone <Cloning Repo URL>
    ```

2. Check which repository you are currently working with:
    ```sh
    git remote -v
    ```

3. Check for all branches in the repository:
    ```sh
    git branch -a
    ```

4. Set the URL of the origin to your own repository (replace `<Your own Repo>` with the URL of your repository):
    ```sh
    git remote set-url origin <Your Own Repo URL>
    ```

5. Verify that the origin URL has been updated:
    ```sh
    git remote -v
    ```

6. Verify for all branches in your repository:
    ```sh
    git branch -a
    ```

Now, your local repository is configured to push changes to your own repository.


