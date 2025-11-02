# algo tri

## installation

### requirements

- SDL3
- pkg-config (for the flags)

```bash
sudo apt install sdl3 pkg-config    # brew or pacman or smth else
```

### repo clone

```bash
git clone git@github.com:Skyleeze/Sort-Algorithm-Viewer.git
```

### compile

compile using cmake.   
note there is no need to use the `cmake` command if [CMakeLists](./CMakeLists.txt) remains unchanged. 

```bash
cd build/
cmake ..
make
```
run the app
```bash
./application
```

### compile (old)

give the execution permission and execute the file

```bash
chmod +x compile.sh
./compile.sh
```
