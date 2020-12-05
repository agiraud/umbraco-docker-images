# umbraco-docker-images

In this repository you will find a set of docker container support files to get up Umbraco demos into docker containers.

All the images for these demos are hosted in public dockerhub registries and are 100% free to access and use [https://hub.docker.com/u/antuangiro](https://hub.docker.com/u/antuangiro).

## Available Umbraco Demo

* **Umbraco 8.9.1 with starterkit**:   
Basic Umbraco instance with the default starterkit package installed, see [https://our.umbraco.com/packages/starter-kits/the-starter-kit/](https://our.umbraco.com/packages/starter-kits/the-starter-kit/).
* **Umbraco 8.9.1 with Vendr demo eCommerce**  
Umbraco instance with [Vendr](https://vendr.net/) demo eCommerce package installed, see [https://github.com/vendrhub/vendr-demo-store](https://github.com/vendrhub/vendr-demo-store)
* **Umbraco 8.9.1 with MarketingSuite**  
Umbraco set up with the starterkit and the [MarketingSuite](https://www.umarketingsuite.com/) package installed (License are needed). 

## Pre-Requisites

1. To use the images from this repository you will need Docker for windows install in your environment and switch it to using Windows containers. If you are new with Docker, refer first to this documentation: [https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/).

2. Then, clone the repository or download it in your local machine.

## Get start using the Docker Images

1. Open a powershell console and go to the path of the demo folder you would like to run:
    - Umbraco starterkit: `/samples/Starterkit`
    - Umbraco Vendr: `/samples/Vendr`
    - Umbraco Marketingsuite `/samples/MarketingSuite`
    - Run of them: `/samples/All`
2. From here, run `docker-compose up -d`  
The first time, the operation will take some time because the images are downloaded into your local environment, but the next time will take some few second.
3. You can now browse the demo in your browser:
    - Umbraco starterkit: [http://umbracodemo.starterkit.local](http://umbracodemo.starterkit.local)
    - Umbraco Vendr: [http://umbracodemo.vendr.local](http://umbracodemo.vendr.local)
    - Umbraco Marketingsuite: [http://umbracodemo.marketingsuite.local](http://umbracodemo.marketingsuite.local)
    
    To login to the back office use the credentials:
    - **Email** admin@admin.com
    - **Password** password1234
    
    **Note:** To use the Umbraco Marketingsuite demo, you need to add a valid license `uMarketingSuite.License.config` into the folder uMarketingSuiteConfig into the demo path. Check in the MerketingSuite website: [https://www.umarketingsuite.com/](https://www.umarketingsuite.com/)
4. You can stop the container with `docker-compose stop` and start it again with `docker-compose start`
5. Remove the container with `docker-compose down`

## URL set up
Modify the default url into the `.env` environement files you can find into the demo folders.
* `HOST_STARTERKIT=umbracodemo.starterkit.local`
* `HOST_VENDR=umbracodemo.vendr.local`
* `HOST_MARKETINGSUITE=umbracodemo.marketingsuite.local`



    





