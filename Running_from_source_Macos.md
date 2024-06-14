How to Run on MacOS :

https://docs.brew.sh/Homebrew-and-Python

TBC : 
```zsh
brew install python3
```

Clone the VU Server repository and install project dependencies

```zsh
python3 -m venv path/to/venv
source path/to/venv/bin/activate
python3 -m pip install -r requirements.txt
```

Run server :
```zsh
python3 server.py 
```

Run example :
```zsh
for i in {1..10}; do shuf -i 0-100 -n 1 | xargs -I{} curl -q "http://localhost:5340/api/v0/dial/500075000750524834313020/set?value={}&key=cTpAWYuRpA2zx75Yh961Cg" && sleep 2 ; echo  && sleep 0.5; done
```



