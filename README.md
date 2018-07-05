**1. Clone wallet sources**

```
git clone https://github.com/cryptonotefoundation/cryptonotewallet.git
```

**2. Modify `CryptoNoteWallet.cmake`**
 
```
set(CN_PROJECT_NAME "scordite")
set(CN_CURRENCY_DISPLAY_NAME "Scordite")
set(CN_CURRENCY_TICKER "XSD")
```

**3. Set symbolic link to coin sources at the same level as `src`. For example:**

```
ln -s ../scordite scordite
```

Alternative way is to create git submodule:

```
git submodule add https://github.com/cryptonotefoundation/cryptonote.git cryptonote
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
