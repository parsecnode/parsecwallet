![image](https://github.com/parsecnode/parsec-icons/blob/main/PARSEC-zero_banner.png?raw=true)

This repository depends on: https://github.com/parsecnode/parsec.git
If you are not running or have not compiled a Parsec Node use the above git hub directory to clone:
sudo git clone https://github.com/parsecnode/parsec.git

BUILDING PARSEC WALLET

**1. Clone wallet sources**

```
git clone https://github.com/parsecnode/parsecwallet.git
```

**2. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ~/parsec/cryptonote ~/parsecwallet/
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/parsecnode/parsec.git cryptonote
```
**3. Install Dependencies**

```
sudo apt install qttools5-dev-tools qttools5-dev
```

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
```
BUILD FILES WILL BE LOCATED WITHIN THE FOLLOWING DIRECTORY: ~/parsecwallet/build/
  *Run Parsec Wallet (linux) in command line: ./ParsecWallet 
```
