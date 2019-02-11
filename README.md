**1. Clone wallet sources

```
git clone https://github.com/scordite/scorditewallet.git
```

**2. Create a git submodule at the same level as src. For example:

```
git submodule add https://github.com/scordite/scordite.git cryptonote
```

**3. Build

```
mkdir build && cd build && cmake .. && make
```

**You can use the scorditewallet for other Cryptonote based currencies:


**1. Clone wallet sources**

```
git clone https://github.com/scordite/scorditewallet.git
```
Replace URL with git remote repository of your coin.

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "scordite")
set(CN_CURRENCY_DISPLAY_NAME "Scordite")
set(CN_CURRENCY_TICKER "XSD")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../scordite cryptonote
```
// Replace "../scordite" with your coin name.

*Alternative way is to create git submodule:

```
git submodule add https://github.com/scordite/scordite.git cryptonote
```
// Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
