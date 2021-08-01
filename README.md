# Conda isntallation in Mac M1.

Since Anaconda is not Apple Silicon (i.e. ARM processor) compatibl; therefore, [Miniforge](https://github.com/conda-forge/miniforge) can be installed which has Conda. 

## First Install [Brew](https://brew.sh)

Run in the terminal
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

After the installation:
```
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/sishirkalita/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## Now, install [Miniforge](https://github.com/conda-forge/miniforge)
```
brew install miniforge
```

### Initialize conda
```
conda init zsh
```

### Create conda env
```
conda create -n macml python=3.8
````

### Environment location: 
```
/opt/homebrew/Caskroom/miniforge/base/envs/macml
```

```
conda activate macula
```

## Install required packages:
```
conda install notebook -y
conda install matplotlib -y
conda install pandas -y
conda install scikit-learn -y 
```
