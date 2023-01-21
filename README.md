# react-native-localstorage
None async local storage based from https://www.npmjs.com/package/react-native-sync-localstorage

## [Installation]
    npm install --save react-native-sync-localstorage-module @react-native-async-storage/async-storage
Or
    {yarn add react-native-sync-localstorage-module @react-native-async-storage/async-storage}

## [Usage]

### 1. Loading stored values at beginnig
    import localStorage from 'react-native-sync-localstorage-module'

    ...

    localStorage.getAllFromLocalStorage()
      .then(() => {
        // Do Something after loading...
      })
      .catch(err => {
        console.warn(err)
      })

### 2. Use local storage comfortable
#### 2-1. Setting
    const value = 12345
    localStorage.setItem('key', value)

#### 2-2. Getting
    localStorage.getItem('key')

#### 2-3. Deleting
    localStorage.removeItem('key')