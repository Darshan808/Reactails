## Docker Development Environment

---

### Windows
**Prerequisites**
|  Name | Version | Installation |
| --- | --- | --- |
| Git | Latest | [Download & Install](https://git-scm.com/downloads) |
| Docker | Latest | [Follow this guide to install](https://docs.docker.com/desktop/install/windows-install/) |

**Steps to setup**
1. Fork current repository
2. Clone the forked repository
    ```bash
    git clone git@github.com:<username></username>/Reactails.git --recursive
    ```
    - Use `git submodule update --init` to get the contents of the submodule if you missed using the `--recursive` option while cloning the repository or if you have already done so.
3. Open `Reactails` directory
4. Open `PowerShell` in the current directory
5. Run `cd server` to navigate in the server directory
6. Run `docker-compose up --build` to start the server through docker
7. Wait for the docker container to be prepared
8. Run `cd ../client` to navigate in the client directory
9. Run `docker-compose up --build` to start the client through docker
   (Or you may run through `npm install` and `npm run dev`)
10. Navigate to `http://localhost:5173` in your browser

**Steps to create a PR**
1. Make required changes in specific directory
2. Open `PowerShell` in that current directory
3. Run `git add .`, commit and push the changes to the repo.
4. Run `cd ..` to navigate to main directory
5. Run `git add .`, commit and push the changes to main repo.
