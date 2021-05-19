# Yarn - Package Manager


- Install via npm

        npm install --global yarn

-  You will first need to configure the repository:

        curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
        echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

- Then you can simply:

        sudo apt update && sudo apt install yarn

- If using nvm you can avoid the node installation by doing:

        sudo apt update && sudo apt install --no-install-recommends yarn

-  Check that Yarn is installed by running: 

        yarn --version
