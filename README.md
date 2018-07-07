**1. Clone wallet sources**

```
git clone https://github.com/scordite/scorditewallet.git
```

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

Alternative way is to create git submodule:

```
git submodule add https://github.com/scordite/scordite.git scordite
```

Replace URL with git remote repository of your coin.

**4. Build**

```
mkdir build && cd build && cmake .. && make
```
