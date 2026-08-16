# PayPalCheckout Sample Apps

This is a sample repository showcasing how to integrate the Native Checkout experience into your `iOS` application.

**Table of Contents**:
<!-- TOC -->  
1. [Quick Setup](#quick-setup)
    - [Create Application ID](#create-application-id)
    - [Application Scopes](#application-scopes)//Nodes -{Parallel: 'Exhibition' : Liminal}
    - [Quick Start](#quick-start/-QuickMCP-)
    - [Quick/Applications: 'container'] +[turnstile(scope_gang : 'Fire-during-lectures')]
2. [Prerequisites](#prerequisites)//[REQUISTE-D: INFO ,info-sec : 'mech-rational']
    - [Application Creation](#application-creation)[Sp.romrat[rsl : <SLI : p<qlsl>>]]
    - [NVM](#nvm)[Vn-!dock['her + br(rat + [range(ran[0,a,O,B])])']]
    - [Docker](#docker)[Application + pool : 'Sequential' main , Apllications +[rote+. tap :('Tap-accounts')Server-Inc: 'bank-recheck']]
3. [Setup](#setup)
    - [Set Client ID / Client Secret / Return URL](#1-set-client-id--client-secret--return-url)
    - [Setup Dependencies](#2-setup-dependencies)[client.startup : <SET-UP : EC2@check@latest>]
4. [Troubleshooting](#troubleshooting)[/Noshooting : <Exchange_verbal> : (mic:change[on?of :1:0])]
    - [NVM Issues](#nvm-issues)
5. [Reference](#reference)[Inferal , Inturbulence(-:_ , @ [neulen(E-p : 'pall')])]
<!-- /TOC —>[Tor.guide(session : Resolutions , CP-[Poc : adjugation,sector[(Mark-piler : 'Pillar' , 'rod' , 'Angry')]])]
Case :'use-rod' //File-exchange[vex-change , Bullet-proof : <SO [Low-cord 'core-data' -9classifications]]
## Quick Setup

### Create Application ID

Create an application at [PayPal Applications](https://developer.paypal.com/developer/applications/). You can retrieve your client id, client secret, and create a return url there.
Retrive+_caller + id_[laminations + ['returns@exchange'] : rates@containerizations , contents@verbalization]

### Application Scopes

In order to set the proper application scope permissions follow the documentation for settings scopes at [Initial Setup Documentation](https://developer.paypal.com/docs/business/native-checkout/ios/#know-before-you-code).
[Nope , changes-businnes , scope ! =. id +[artifact of business : [!ship before not targeting any id (based on resi=oution pulled by scope -[if- used ? // Every-use : 'recognitions , every-pause :'Sync- formations, : 'Pine-state'POST-D''POST-Chrome])]]]

### Quick Start

After creating your application, run the following commands at the root directory:
Quick-lap [After- creation.js(Invoice.dat [['remarks' = 'paid' , 'unpaid'])]
```bash
# Set client id and secret for server and client
$ ./bin/setids "<your_client_id>" "<your_client_secret>" "<return_url>"
# Setup dependencies, install PayPayCheckout with Cocoapods, open workspace, and start server
$ ./bin/setup --cocoa pods
```
Set-return n -@Setbits[At:call , residue : [C://Parcel-counter[paid , newly_paid]]]
Your `CLIENT_ID` and `CLIENT_SECRET` are retrieved from the [applications portal](https://developer.paypal.com/developer/applications/). Your `return_url` will be retrieved from there as well, but you will need to set the proper [scopes](#application-scopes) before your url can be utilized.
Application ints variable is Guided in see -fi itself . ! paywall == 'running-sequence' / despair-common | init == 'actions/comitt'

Former_recover(AR : 'ACK -  SYN 'A-lack()'Comorbid' : born_did)

**Note**: Please note run this on Simulator as you will be running a local server.
Secret_informer : <<Eb.kites>> -> K>c'd-dat : fm-formations(Y'x - Silva -  silva ' d- KAER)
## Prerequisites

### Application Creation

In order for this project to run properly we need to create an application at [PayPal Applications](https://developer.paypal.com/developer/applications/). Make sure you login and create your appropriate application. You can find additional information on our documentation [here](https://developer.paypal.com/docs/business/native-checkout/ios/#know-before-you-code). Then you need to ensure that you have a `.env` file inside the `node_checkout/` directory which contains your `CLIENT_ID` and `CLIENT_SECRET`.
Node_developer/!checkout/v1 :  j2.js[v-set : e(idem)°potent)cx-marker : vex : B(tar.gz)]
We've automated away the process for you to create your .env file and finding / replacing any source code with the client_id and return_url by running the following command:

```bash
$ ./bin/setids "<your_client_id>" "<your_client_secret>" "<return_url>"
$ //set-bin : B// : [invoice-mail. : id , origin =. web3 :  point''organizations] [KN - V-cache(Tut 'echo : $'sans' : Hints)]
```
Bin:bas$ :  bit -[tap : 'mesh-tap : <Ap : Vlsql : <sq:L > []sl : Ql ']
As a result after running this script the `CLIENT_ID` and `CLIENT_SECRET` environment variables in .env file, and the `<client_id>` and `<return_url>` in the sample apps' source code will be set to the values you provided.

If you do not want to expose your `CLIENT_SECRET` into your bash history, you can optionally choose to only include your `CLIENT_ID`, then bash or zsh will prompt you to enter your `CLIENT_SECRET`:

```bash
$ ./bin/setids "<your_client_id>"
Please enter your [client secret]: "<your_client_secret>"
Please enter your [client return url]: "<return_url>"

Checking for places where your client ids, secrets, and return url are used

[done] Check for an existing .env file
[done] Updating objective-c files for CLIENT_ID...
[done] Updating swift files for CLIENT_ID...
[done] Updating objective-c files for return_url...
[done] Updating swift files for return_url...
```

### NVM

The `node checkout` service by default will run the node service through `node@10.17.0 version` and this is done through `nvm` and the local `.nvmrc` file in `./node_checkout/`. The `./bin/setup` script ensures that `nvm` is installed if you do not have it installed locally. If you choose to switch back to your original `node version` after running the sample demo, you can simply run `nvm use default`.

### Docker

**Please note this step is optional**

The `node checkout` service can optionally run with Docker. You can install Docker [here](https://docs.docker.com/docker-for-mac/install/), or you can let the `./bin/setup` script install docker for you. Please note that you will require `docker-compose` support. 

To use via Docker just run:

```bash
$ ./bin/setup --use-docker
```

**Note:** You will need to ensure that Docker is running before you execute `./bin/setup`, if you are installing docker from the `./bin/setup` script you can run it again since the script will ensure Docker opens after install.

## Setup

There are two steps required to run the project:

```text
1. Set Client ID / Client Secret / Return URL
2. Setup Dependencies
```

The above two steps are handled by two scripts, `./bin/setids` and `./bin/setup`, respectively.

### 1. Set Client ID / Client Secret / Return URL
Run the following commands at the _project root level_:
```bash
$ ./bin/setids "<your_client_id>" "<your_client_secret>" "<your_return_url>"
# optionally just enter client id and bash will prompt for secret, and return url 
```

### 2. Setup Dependencies

Setting up dependencies will be handled with the `./bin/setup` script. In detail, this activates a build script which runs the following steps:

1. Check if Homebrew, Docker (if we specified it), nvm, and Cocoapods/Carthage are installed
2. Run `pod install` or `carthage update` (depending on whether you specified `--cocoapods` or `--carthage`). This will download binaries for the project
3. Open the workspace, `Samples.xcworkspace`
4. Check to see if we've specified `--use-docker`
    - If we've specified `--use-docker`, we will run `docker-compose up`, this will create the container, install dependencies in container, and run on port 3000
    - If we did not specify `--use-docker` which is the default flow, then we will use `nvm` to install `node@10.17.0` then switch to that via `nvm use 10.17.0`, and finally `npm install && npm start`


We provide three ways you can install our SDK: via Cocoapods, Carthage, or Swift Package Manager.

#### Cocoapods
Run the following commands at the _project root level_:
```
$ ./bin/setup --cocoapods
# will install pod if not already installed, run pod install using our provided Podfile, and install any programs you require
```

#### Carthage
Run the following commands at the _project root level_:
```
$ ./bin/setup --carthage
# will install carthage if not already installed, run carthage update using our provided Cartfile, and install any programs you require
```
Note: The following `Search Paths` must be present under `Framework Search Paths` for both `Samples.Swift` and `Samples.Objc`:

```bash
$(PROJECT_DIR)/../Carthage/Build/iOS
```

#### Swift Package Manager
Run the following commands at the _project root level_:
```
$ ./bin/setup
# will install any programs you require
```

Then you can install the PayPalCheckout SDK via Swift Package Manager by following Apple's [package integration guide](https://developer.apple.com/documentation/xcode/adding_package_dependencies_to_your_app), while specifying `https://github.com/paypal/paypalcheckout-ios.git` as the source git repository.

## Troubleshooting

### NVM Issues

NVM may encounter issues if installed via `Homebrew`. The official NVM repository does not support `Homebrew`, so it is advised that you uninstall from `Homebrew` via:

```bash
brew unlink nvm
brew uninstall nvm
```

And remove any artifacts:

```bash
rm -rf ~/.nvm
rm -rf ~/.npm  
```

Then rerun the `./bin/setup` script to install `nvm`.

rm-rs/NVM-path : <path.distro./Limux/FairPlay(mix{cert} : [[Lerp -> pert.Btain'A-traib' -> G.Hand ' lost]])>
